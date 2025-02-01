# UG Speech Data - Ewe (Dataset Split)

This repository contains the dataset split used for training the Ewe Automatic Speech Recognition (ASR) model based on the UG Speech Data dataset.

## Dataset

The original UG Speech Data dataset can be found on DropBox Face: https://www.dropbox.com/scl/fo/e9bha9glyvk2mu5fo7f3h/h/Ewe?dl=0&subfolder_nav_tracking=1.

This repository provides the split of this dataset into training, testing, development, and secret sets.

## Files

- `train_data.xlsx`: Contains the metadata for the training set.
- `test_data.xlsx`: Contains the metadata for the testing set.
- `dev_data.xlsx`: Contains the metadata for the development set.
- `secret_data.xlsx`: Contains the metadata for the secret set.

Each Excel file contains the following columns:

- **Full Filename**: Name of the audio file.
- **SPEAKER_ID**: Unique identifier for the speaker.
- **GENDER**: Gender of the speaker (Male/Female).
- **AGE**: Age of the speaker.
- **ENVIRONMENT**: Environment where the audio was recorded (e.g., Home, Office).
- **DEVICE**: Device used for recording (e.g., Smartphone, Microphone).
- **Transcription**: Text transcription of the audio.

## Splitting Criteria

The dataset was split using the following criteria:

- **Training Set (70%)**: Used to train the ASR model.
- **Testing Set (20%)**: Used to evaluate the model's performance on unseen data.
- **Development Set (8%)**: Used for hyperparameter tuning and model selection.
- **Secret Set (2%)**: Kept aside for final evaluation to avoid overfitting to the test set.

The splitting was done based on speaker IDs to ensure no speaker overlap between the sets.

## Usage

You can use these split datasets to train and evaluate your own Ewe ASR models.

1. Download the Excel files from this repository.
2. Load the data into your training pipeline.
3. Adjust the paths to the audio files in the metadata accordingly.

## License

The license for the UG Speech Data dataset can be found on the original dataset at [speech_data_ghana_ug](https://github.com/HCI-LAB-UGSPEECHDATA/speech_data_ghana_ug). Please refer to that page for licensing details.

## Citation

If you use this dataset split in your work, please cite the original UG Speech Data dataset and this repository.
