<div align="center" markdown>

<img src="" style="width: 100%;"/>

# Template Serve NN Detection

<p align="center">
  <a href="#overview">Overview</a> •
  <a href="#preparation">Preparation</a> •
  <a href="#how-to-use">How To Use</a> •
  <a href="#how-to-add-model-as-app-enterprise-edition-only">How To Add Model As App</a> •
  <a href="#how-to-run">How To Run</a> •
  <a href="#related-apps">Related Apps</a> •
  <a href="#result">Result</a>
</p>


[![](https://img.shields.io/badge/supervisely-ecosystem-brightgreen)](https://ecosystem.supervise.ly/apps/supervisely-ecosystem/template-serve-nn-detection)
[![](https://img.shields.io/badge/slack-chat-green.svg?logo=slack)](https://supervise.ly/slack)
![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/supervisely-ecosystem/template-serve-nn-detection)
[![views](https://app.supervise.ly/public/api/v3/ecosystem.counters?repo=supervisely-ecosystem/template-serve-nn-detection&counter=views&label=views)](https://supervise.ly)
[![used by teams](https://app.supervise.ly/public/api/v3/ecosystem.counters?repo=supervisely-ecosystem/template-serve-nn-detection&counter=downloads&label=used%20by%20teams)](https://supervise.ly)
[![runs](https://app.supervise.ly/public/api/v3/ecosystem.counters?repo=supervisely-ecosystem/template-serve-nn-detection&counter=runs&label=runs&123)](https://supervise.ly)

</div>

# Overview

Template Serve NN Detection app is designed for **developers** and can be used as a starting point for creating an application for serving your own detection NN models on Supervisely.

By default template app generates random predictions with random scores to demonstrate the functionality, in order to implement your custom model, you will need to edit **`main.py`**. Inference results will be automatically converted to [supervisely annotation format](https://docs.supervise.ly/data-organization/00_ann_format_navi).

# Preparation

**Step 1.** Make a fork from this repository

**Step 2.** Download it to your computer

# How To Use

**Note:** recommended Python version for supervisely is 3.8.x

**Step 1.** Create python virtual environment by running the following command from the application root directory in terminal:

```bash
python -m venv venv
```

**Step 2.** Activate virtual environment:

```bash
source venv/bin/activate
```

**Step 4.** Install requirements.txt:

```bash
pip install -r requirements.txt
```

**Step 5.** Make sure you've edited `main.py`, without edits it will generate random predictions

**Step 6.** Run `main.py` from terminal or by using your IDE interface:

```bash
python main.py
```

**Step 7.** When your model is ready, add additional modules that are required to run your served model to requirements.txt

**Step 8.** Add your model as private app to Supervisely Ecosystem

# How To Add Model As App [Enterprise Edition only]

**Step 1.** Go to Ecosystem page and click on `private apps`

<img src="" style="width:100%;"/>

**Step 2.** Click `+ Add private app` button

<img src="" style="width:100%;"/>

**Step 3.** Copy and paste repository url and generated [github/gitlab personal token](https://docs.supervise.ly/enterprise-edition/advanced-tuning/private-apps) to modal window

<img src="" style="width:100%;"/>

# How To Run:

**Step 1.** Add [Template Serve NN Detection](https://ecosystem.supervise.ly/apps/supervisely-ecosystem%252Ftemplate-serve-nn-detection) to your team from Ecosystem

<img src="" style="width:100%;"/>

**Step 2.** Run the application from the context menu of `.pth` file. If you are running application from file with different than `.pth` extension, app will use default model with random predictions.

<img src="" style="width:100%;"/>

**Step 3.** Press the Run button in the modal window

<img src="" style="width:100%;"/>

**Step 4.** Add one of the [related apps](https://github.com/supervisely-ecosystem/template-serve-nn-detection/edit/dev-readme/README.md#related-apps) to your team from Ecosystem and run it.

**Step 5.** Open running applier app and connect to app session with served model

<div>
  <table>
    <tr style="width: 100%">
      <td>
        <b>NN Image Labeling</b>
        <img src="" style="width:100%;"/>
      </td>
      <td>
        <b>Apply NN to Images Project</b>
        <img src="" style="width:100%;"/>
      </td>
    </tr>
  </table>
</div>

**Step 6.** Apply NN model to image or whole project/dataset

<div>
  <table>
    <tr style="width: 100%">
      <td>
        <b>NN Image Labeling</b>
        <img src="" style="width:100%;"/>
      </td>
      <td>
        <b>Apply NN to Images Project</b>
        <img src="" style="width:100%;"/>
      </td>
    </tr>
  </table>
</div>


# Related apps

Learn how to use served models in the corresponding apps:

* [NN Image Labeling](https://ecosystem.supervise.ly/apps/supervisely-ecosystem%252Fnn-image-labeling%252Fannotation-tool) - **Apply served model to image** 
* [Apply NN to Images Project](https://ecosystem.supervise.ly/apps/supervisely-ecosystem%252Fnn-image-labeling%252Fproject-dataset) - **Apply served model to whole project or dataset**

# Result

<img src="" style="width:80%;"/>



