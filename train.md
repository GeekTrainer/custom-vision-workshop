# Train

## Create the project

Describe here

1. Navigate to [Custom Vision](https://www.customvision.ai)
1. Select **New Project**
1. Enter **Dog Classification** for the project name
1. Next to Resource, select **create new** to create a key in Azure for the service
1. On the **Create New Resource** enter the following information
    - **Name**: **custom-vision**
    - **Subscription**: Choose your student subscription
    - **Resource Group**: Select **Create New**
        - Enter **custom-vision** for the name, and choose a location near you, then select **Create resource group**
        - Select the **custom-vision** resource group you created
    - **Kind**: **CustomVision.Training**
    - **Location**: The same location you chose earlier
    - **Pricing Tier**: **F0** for the [free tier](https://docs.microsoft.com/azure/cognitive-services/custom-vision-service/limits-and-quotas)
    - Select **Create resource**
1. For **Project Types** select **Classification**
1. For **Classification Types** select **Multiclass**, as our dogs will only have one breed
1. For **Domains** select **General**
1. Select **Create project**

## Upload images

Once the project is created it's time to upload images.

1. Select **Add images**
1. Navigate to **folder**
1. Select all the images marked as **american-staffordshire-terrier** in the folder, and select **Open**
1. Enter **american-staffordshire-terrier** for the tag and select **Upload 8 files**
1. Select **Done**
1. Repeat the above steps for the remaining breeds:
    - **australian-shepherd**
    - **buggle**
    - **german-wirehaired-pointer**
    - **shorkie**
1. Select **Train** to open the training dialog
1. Leave **Quick Training** selected and select **Train** to begin the training process

Training will take a little bit.

## Test the model

With the model trained, let's see how well it works.

1. Select **Quick Test**
1. Select **Browse local files**
1. Navigate to **FOLDER** and select one of the dog images
1. Select **Open**
1. Notice the **tag** and **probability** scores
