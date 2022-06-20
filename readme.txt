This is the accompanying readme file for Applied AI CA3:

Firstly, there are two notebooks attached:

VGG Testing - This notebook includes our enhancement of the VGG model.

ResNet Testing - This notebook includes the enhancement of the ResNet model and also is the main file for this assignment.

When observing the visualisation for the data, the ResNet notebook contains items such as the image samples and classification reports for part 1 of the assignment

The reason two were included, we felt testing the pre-trained alone was not effective in picking a winner, due to how the results may fluctuate a bit.

The google colab notebooks offer simplicty when running our code, with just pressing start on the tabs 

To load the data initally, the following method was utilised:



'''
    login to Kaggle and access account,

    create "new api token" - this will download a .json file,

    next - save the .json file to a google drive account,
    
    to access google drive the below command is in the notebooks: 
    
    from google.colab import drive
    drive.mount('/content/gdrive')

    this will then create a prompt to authorise, so that the drive can be accessed.

    next - following command is used to create an environment to utilise the kaggle.json and it's features:

    import os
    os.environ['KAGGLE_CONFIG_DIR'] = "/content/drive/MyDrive/kaggle-2.json


    finally, to load the dataset for this assignment, the below command is used:

    !kaggle datasets download -d prashant268/chest-xray-covid19-pneumonia

    alongside an unzipping of the file, in order to fully access it:

    !kaggle datasets download -d prashant268/chest-xray-covid19-pneumonia --unzip --force'''


With the above cells ran and the .json file downloaded, the notebook can now run and the dataset should appear in the left hand side of the files section in colab.

To reproduce the results of our report/assignment, all that must be done now is running the individual cells, which do not require any editing prior to running

