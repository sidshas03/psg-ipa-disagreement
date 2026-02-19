# PSG-IPA Colab Project

This project provides a Colab-ready notebook for disagreement-aware sleep scoring on PSG-IPA.

## File

- `psg_ipa_disagreement_aware_colab.ipynb`

## What it does

- Downloads the `Sleep_stages` portion of PSG-IPA.
- Reads raw PSG and scorer annotations.
- Builds 30-second epoch features.
- Computes per-epoch inter-scorer disagreement from multiple scorers.
- Trains:
  - a sleep stage classifier
  - an ambiguity-risk classifier
- Applies a triage rule:
  - auto-accept high-confidence / low-risk epochs
  - flag uncertain epochs for human review

## Run in Colab

1. Upload the notebook to Google Colab.
2. Run cells top-to-bottom.
3. Outputs are saved under `/content/psg_ipa_project/results`.

## Notes

- Default configuration downloads up to 5 recordings for the selected task.
- You can expand to all tasks (`EEG_arousals`, `Limb_movements`, `Resp_events`) by adapting label logic.

## Dataset

PSG-IPA on PhysioNet:

- https://physionet.org/content/psg-ipa/1.0.0/

## License

- Project code/notebooks: MIT (see `LICENSE`)
- Dataset files: remain under PSG-IPA/PhysioNet terms (CC BY 4.0), see `DATASET_LICENSE_NOTICE.md`
