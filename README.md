<div align="center" markdown>

<img src="" style="width: 100%;"/>

# Template Serve NN Detection

<p align="center">
  <a href="#Overview">Overview</a> •
  <a href="#How-To-Run">How To Run</a> •
  <a href="#Related-Apps">Related Apps</a>
</p>


[![](https://img.shields.io/badge/supervisely-ecosystem-brightgreen)](https://ecosystem.supervise.ly/apps/supervisely-ecosystem/template-serve-nn-detection)
[![](https://img.shields.io/badge/slack-chat-green.svg?logo=slack)](https://supervise.ly/slack)
![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/supervisely-ecosystem/template-serve-nn-detection)
[![views](https://app.supervise.ly/public/api/v3/ecosystem.counters?repo=supervisely-ecosystem/template-serve-nn-detection&counter=views&label=views)](https://supervise.ly)
[![used by teams](https://app.supervise.ly/public/api/v3/ecosystem.counters?repo=supervisely-ecosystem/template-serve-nn-detection&counter=downloads&label=used%20by%20teams)](https://supervise.ly)
[![runs](https://app.supervise.ly/public/api/v3/ecosystem.counters?repo=supervisely-ecosystem/template-serve-nn-detection&counter=runs&label=runs&123)](https://supervise.ly)

</div>

# Overview

Template Serve NN Detection app is designed for **developers** and can be used as a starting point for creating an application for serving your own custom NN models on Supervisely.

By default template app generates random predictions with random scores to demonstrate the functionality, but you will need to replace implementation of the [`generate_predictions()`](https://github.com/supervisely-ecosystem/template-serve-nn-detection/blob/eb45fde8eab536a4acb3023b97ab111885ec1e48/src/helpers.py#L38) function in [`src/helpers.py`](https://github.com/supervisely-ecosystem/template-serve-nn-detection/blob/dev-readme/src/helpers.py) on your own, using the inference of your own model. Inference results will be automatically converted to [supervisely annotation format](https://docs.supervise.ly/data-organization/00_ann_format_navi).

We prepared scripts in [`src`](https://github.com/supervisely-ecosystem/template-serve-nn-detection/tree/dev-readme/src) directory and example [`custom_settings.yaml`](https://github.com/supervisely-ecosystem/template-serve-nn-detection/blob/dev-readme/custom_settings.yaml) file to help you:

* **src/sly_globals.py** - contains essential variables and supervisely app initialization.
* **src/main.py** - contains handlers for communicating with **NN applying** application.
* **src/helpers.py** - contains scrpits for model inference
* **custom_settings.yaml** - contains settings for post-processing and designed to store parameters.

# How To Run

**Step 1.** Add [Template Serve NN Detection](https://ecosystem.supervise.ly/apps/supervisely-ecosystem%252Ftemplate-serve-nn-detection) to your team from Ecosystem

**Step 2.** Run the application from `Plugins & Apps` page

**Step 3.** Press the Run button in the modal window

# Related apps

Learn how to use served models in the corresponding apps:

* [NN Image Labeling](https://ecosystem.supervise.ly/apps/supervisely-ecosystem%252Fnn-image-labeling%252Fannotation-tool) - **Apply served model to image** 
* [Apply NN to Images Project](https://ecosystem.supervise.ly/apps/supervisely-ecosystem%252Fnn-image-labeling%252Fproject-dataset) - **Apply served model to whole project**

# How To Debug

**Step 1.** Run one of the related apps on Supervisely instance.

**Step 2.** Configure environment variables and run the app locally from your favorite IDE. Learn more about supervisely applications [here](https://github.com/supervisely-ecosystem/how-to-create-app)

**Step 3.** Connect to served model by Task ID

**Step 4.** Apply model 
