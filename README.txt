The code for our project is a notebook intended to be run with
Google Colab.  Training the model takes a long time, so we provide
several pre-trained models along with the notebook file.

To run with pre-trained models:

0. Ensure you are connected to a GPU runtime on Colab and using one of
   the supported GPUs (see comment in first cell).
1. Edit the cell under the "Constants" heading at the top, and set
   data_category to either "cars" or "chairs".
2. Under "Directories & downloading data", set GDRIVE_ENABLED to False.
3. Merge the contents of the "local" folders from "Pretrained_chairs.zip" and
   "Pretrained_cars.zip" to the path "<files>/local" in Colab storage.
4. Run all cells one by one up to the end of the "Setup" subsection of "Training".
5. There are several headings that look like "Restore State ..." and
   include the model name in the heading.  To load a model, run the first
   cell under a given heading.  This will restore the model state from
   the pre-trained model file.
6. Run the relavant cells under the "Evaluation" heading to show the model
   output and compute evaluation statistics.

Due to memory limitations, we advise not to load all models at once.
