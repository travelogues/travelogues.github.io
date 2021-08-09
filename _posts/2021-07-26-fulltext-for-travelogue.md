| title | share | permalink |
| ----  | ----  | ---- |
| Images and fulltext for travelogue | true | /2021-07-26-fulltext-for-travelogue |

>**Note**: This post offers a description for how to download images and fulltext for a single travelogue of our corpus, if you are not familiar with the *Austrian National Library's* programming interface (API) [SACHA](https://iiif.onb.ac.at). If you are interested in images or fulltexts for the whole Travelogues-corpus, please contact our team. 

## How to get the images of a digitized travelogue ##

In our post [Searching for Travelogues](https://travelogues-project.info/2021-04-21-searching-for-travelogues/) we have offered you a guide on how to search for travelogues from the project's corpus in the 
**online public access catalog** (OPAC) [*Quicksearch*](https://search.onb.ac.at/primo-explore/search?vid=ONB&lang=en_US) of the *Austrian National Library* (ONB) and on how to look at the digitized item in the ONB's viewer. In the result list of your Quicksearch query you find a link labeled **"Online access"** for every digitized item. Clicking on this link the viewer will open in a separate browser window. 

![Access digitized item in the ONB Viewer](/images/Fulltext-for-travelogue_Screenshot_1.jpg)

By right-clicking over any page (s. Screenshot), a menu opens up. You may rotate the image to the left or to the right. You may also download either the image of the page currently shown ("Bild herunterladen") or images of the whole book ("Buch herunterladen") as PDF-files.

![Download-menu in the ONB Viewer](/images/Fulltext-for-travelogue_Screenshot_2.jpg)

In the viewer application you can search for any string in the fulltext (e.g. "Pyramide). The results are marked in the text and you can click through the selected result pages in the menu bar (e.g. "Bild 1 von 7 mit Treffern"). 

![Search the fulltext in the ONB Viewer](/images/Fulltext-for-travelogue_Screenshot_3.JPG)

## How to get the fulltext for a travelogue ##

For downloading the fulltext of a single travelogue (i.e. fulltext of one digitized copy) we offer a [Jupyter-Notebook](https://labs.onb.ac.at/gitlab/georgp/sacha-txt-downloader/) named "txt-downloader" in the [*ONB Labs*](https://labs.onb.ac.at/en/) GitLab. To run this tool you do not need to download any software or code, it runs in the browser via my Binder. By running this notebook, you will get a ZIP-folder in the output-repository of the Binder application, which you may download. The ZIP-folder contains plain-text-files for each page plus a text-file, in which all text-files of the single pages are combined into one file. Please note that neither structural metadata for page sequence is contained in the combined text file nor any markup (e.g. page breaks). 


+ First step: Click on [Jupyter-Notebook](https://labs.onb.ac.at/gitlab/georgp/sacha-txt-downloader/)

![Notebook in the ONB Labs GitLabs](/images/Fulltext-for-travelogue_Screenshot_4.JPG)

+ Second step: click on **launch binder**. A Binder instance is being launched in a separate browser window. 

+ Third step: As soon as the Jupyter-Notebook opens you may start the application by clicking on "run all" in the menu "cells". Command blocks (cells) executed will have a counter in front, those not completed an asterisk (/*). 

![Run all cells in Notebook](/images/Fulltext-for-travelogue_Screenshot_5(1).jpg)

+ Forth step: In the second cell - which will be marked by an asterisk as not yet completed - will appear an insert bar. Please enter the barcode in the form of the example given (without dot or space at the end!) and press the Return key. Please read the following note on how to get the barcode!

![Enter barcode](/images/Fulltext-for-travelogue_Screenshot_7.jpg)

>**Note:** Each digitized item is identified by a **barcode** (e.g. *Von der Alster zu den Pyramiden* +Z257607709). For downloading fulltext via the ONB Labs Jupyter-Notebook you have to input the barcode identifier of the item, for which you want to download the fulltext. You can find the barcode in the item overview, which opens by clicking on a single result for your search query in the *Quicksearch* catalog. Please copy the barcode!

![Barcode for digitized item](/images/Fulltext-for-travelogue_Screenshot_6.jpg)

+ Fifth step: Have you pressed the Return key after insertion of the barcode? The download will start for each single txt-file. After the next "In"-block you will see single lines for downloading single txt-files. You can click on any of them, to see the OCR-text for the single page chosen. At the end you will get a link to a ZIP-file "{barcode}.zip" in the "Out"-cell. 

>**Note**: Our travelogues are part of Austrian Books Online (ABO), a public-private partnership of the Austrian National Library with Google Books. You may only use digitized items and fulltexts from ABO by accepting the [right statement](https://rightsstatements.org/page/NoC-NC/1.0/?language=en) for **non commercial use only**. Please also note that you are allowed to use this notebook only for the download of individual barcodes (no bulk download allowed!).

For help or further information please contact our librarian at <martin.krickl@onb.ac.at>.

