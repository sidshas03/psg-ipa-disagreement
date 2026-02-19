# PSG-IPA Dataset Links

Dataset landing page:
- https://physionet.org/content/psg-ipa/1.0.0/

DOI (v1.0.0):
- https://doi.org/10.13026/esx0-nw71

Terminal download (recursive):
- `wget -r -N -c -np https://physionet.org/files/psg-ipa/1.0.0/`

AWS sync:
- `aws s3 sync --no-sign-request s3://physionet-open/psg-ipa/1.0.0/ DESTINATION`

Direct files root:
- https://physionet.org/files/psg-ipa/1.0.0/

## Note for this repository

This repository includes a runnable project subset under `psg_ipa_project/` for demonstration and reproducibility.
For full-scale experiments, download the complete dataset from the links above.
