---
layout: default
title: "SISTR: Salmonella In Silico Typing Resource"
search_title: "SISTR: Salmonella In Silico Typing Resource"
description: "A tutorial on how to type data with SISTR."
---

Typing *Salmonella* data with SISTR
===================================
{:.no_toc}

This is a quick tutorial on how to use IRIDA to analyze data with the [*Salmonella in-silico* Typing Resource (SISTR)][sistr-web].

* TOC
{:toc}

Initial Data
============

The data for this tutorial comes from <https://sairidapublic.blob.core.windows.net/downloads/data/irida-sample-data.zip>. It is assumed the sequence files in `miseq-run-salmonella/` have been uploaded into appropriate samples as described in the [Web Upload Tutorial][]. Before starting this tutorial you should have a project with samples that appear as follows:

![sistr-samples]

Adding Samples to the Cart
==========================

Before a pipeline can be run a set of samples and sequence read data must be selected and added to the cart. For this tutorial please select the single sample and click the **Add to Cart** button.

![add-to-cart]

Once the samples have been added to the cart, the samples can be reviewed by clicking on the **Cart** button at the top.

![cart-button]

Selecting a Pipeline
====================

Once inside the cart all available pipelines will be listed in the main area of the page. For this tutorial, we will select the **SISTR Pipeline**.

![pipeline-select]

Selecting Parameters
====================

Once the pipeline is selected, the next page provides an overview of all the input files, as well as the option to modify parameters. We will use the default parameters.

![sistr-pipeline-page]

Please use the **Launch Pipeline** button to start the pipeline.

![launch-button]

Once the pipeline is launched, you will be redirected to the analysis details page.

Monitoring Pipeline Status
==========================

At any point, to monitor the status of the launched pipeline, please select the **Analysis > Your Analyses** menu.

![view-your-analyses]

This will bring you to a page where you can monitor the status of each launched workflow.

Clicking the pipeline name will bring you to a page for that analysis pipeline. It will take a while for the SISTR analysis pipeline to complete. Along the top of the page you can check the current step of the analysis and at the bottom of the **Details** tab you can select if you would like to receive an email upon pipeline completion or error. The email option is only available if the analysis is not in `COMPLETED` or `ERROR` state.

![analysis-in-progress]

Viewing the Results
===================

Once the pipeline is complete, you will see the SISTR Typing results within your browser. For more details on interpreting the results, please see the [IRIDA SISTR Documentation][].

![sistr-info]

![sistr-cgmlst]

![sistr-mash]

You can view the `sistr` analysis output files in tabular, textual and/or json view. Note that not all files have an available preview and as such are not displayed in the Output File Preview but are downloaded when selecting the `Download All Files` button.

![sistr-output-preview]

To download individual files select the **...** next to the Download All Files and select the file to download.

![sistr-download-individual-files][]

To download all the files generated by the analysis, please select the **Download All Files** button.

![sistr-download-all-files][]


Interpreting the Results
========================

For information on interpreting the SISTR results, please refer to the detailed [SISTR Report Documentation][].

Viewing Provenance Information
==============================

To view the pipeline provenance information, please select the **Provenance** tab.

![sistr-provenance]

The provenance is displayed on a per file basis. Clicking on `sistr-predictions.json` file will display it's provenance. Expanding each tool will display the parameters that the tool was executed with.

![sistr-provenance-tools]


Viewing Pipeline Details
========================

To view analysis details, please select the **Settings** tab. From here you can view the analysis name, analysis description, analysis id, pipeline and pipeline version used by the analysis, analysis priority, when the analysis was created, and duration of the analysis.

![sistr-settings]

To edit an analysis name, please select the Pencil icon next to the analysis name. Once you have edited the analysis name, pressing the `ENTER` key on your keyboard or clicking anywhere outside of the text box will update the name. To cancel editing a name you can either hit the `ESC` key on your keyboard or if the name has not been changed you can also click anywhere outside of the text box.

![sistr-settings-edit-name]

To view samples used by the analysis, please select the **Samples** tab.

![sistr-settings-samples]

To share analysis results with other projects and/or save results back to samples, please select the **Manage Results** tab.

![sistr-settings-share]

To delete an analysis, please select the **Delete Analysis** tab.

![sistr-settings-delete]


[add-to-cart]: images/add-to-cart.png
[analysis-in-progress]: images/analysis-in-progress.png
[cart-button]: images/cart-button.png
[IRIDA SISTR Documentation]: ../../user/sistr/
[launch-button]: ../../../images/tutorials/common/pipelines/ready-to-launch-button.png
[monitor-analyses]: images/monitor-analyses.png
[pipeline-launched]: images/pipeline-launched.png
[pipeline-select]: images/pipeline-select.png
[sistr-info]: images/sistr-info.png
[sistr-cgmlst]: images/sistr-cgmlst.png
[sistr-download-all-files]: images/sistr-download-all-files.png
[sistr-download-individual-files]: images/sistr-download-individual-files.png
[sistr-mash]: images/sistr-mash.png
[sistr-output-preview]: images/sistr-output-preview.png
[sistr-pipeline-page]: images/sistr-pipeline-page.png
[sistr-provenance]: images/sistr-provenance.png
[sistr-provenance-tools]: images/sistr-provenance-tools.png
[sistr-samples]: images/sistr-samples.png
[sistr-serovar-predictions]: images/sistr-serovar-predictions.png
[sistr-settings]: images/sistr-settings.png
[sistr-settings-delete]: images/sistr-settings-delete.png
[sistr-settings-edit-name]: images/sistr-settings-edit-name.png
[sistr-settings-samples]: images/sistr-settings-samples.png
[sistr-settings-share]: images/sistr-settings-share.png
[sistr-web]: https://lfz.corefacility.ca/sistr-app/
[SISTR Report Documentation]: ../../user/sistr/#report
[view-your-analyses]: images/view-your-analyses.png
[Web Upload Tutorial]: ../web-upload/