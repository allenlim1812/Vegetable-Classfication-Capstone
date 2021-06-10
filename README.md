# Vegetable-Classfication-Capstone

## 1 Why is this project important?

The idea behind this project was to break down a large issue into very small parts and solving those small issues one at a time from the ground up. I spent a lot of time thinking of ideas that are current but also have potential business impact.

The problem I chose to dive into was climate change and global warming. There are many factors for climate change and global warming and the most common ones are the burning of fossil fuels, deforestation, and population growth. However, there are other lesser known reasons such as increased agriculture and overfishing. I decided to focus on overfishing as an issue and figure out how to combat this issue.

It is obvious that large scale issues do not have a one size fits all solution so I focused on how we could reduce fish consumption. The simple conclusion I reached was by promoting the consumption of vegetables and produce. Vegetables are very widely available and are inherently healthy to the human body. Howver, the issue with vegetables is that many people do not know the nutrtional value nor how to prepare them.

Thus, I decided on a vegetable image classifier in order to help promote a sustainble and healthy diet in order to reduce the consumption of fish

## Data

There were no readily available datasets of vegetables online and if there were they size or picture qualities of the images contained within them were not big enough.

I resorted to using a scraper I found online to scrape images from google images for each individual class. The goal was to get around 1000 images for each class and have a total of 5 classes to produce my model. However, there were some difficulties with the images scraped from google images.

Upon inspecting my scraped images I ran into several issues. There were many images with watermarks, cartoon images, or images with people in them. Ideally I would have had images of only the vegetable in its rawest form. Though google images is abundant it is not unlimited. After cleaning my dataset of all unwanted images I was only able to get around 400-500 images per class which was not ideal but was still possible to work with

## Modelling

The first model I built using only the images collected with no pre-trained model achieved an accruacy score of 72% after data augmentation. In order to improve this I decided to use the VGG16 pre-trained model after a lot of experimenting with otehr pre-trained models as it yielded the best results. I was able to achieve an 83% accuracy after adding in my own custom layers.

## Improvements

This image classifier could definitely be improved by collecting more accurate and consistent data. Since the images were scraped from google images the size and quality of the images were inconsistent. Furthermore, having images with a more diverse background and consistent object that needed to be detected would help as well to prevent misclassifications.