| title | share | permalink |
| ----  | ----  | ---- |
| Images and fulltext for travelogue | true | /2021-06-23-fulltext-for-travelogue |

>**Note**: This post offers a description for how to download images and fulltext for a single travelogue of our corpus, if you are not familiar with the *Austrian National Library's* programming interface (API) [SACHA](https://iiif.onb.ac.at). If you are interested in images or fulltexts for the whole Travelogues-corpus, please contact our team. 

## How to get the images of a digitized travelogue ##

In our post [Searching for Travelogues](https://travelogues-project.info/2021-04-21-searching-for-travelogues/) we have offered you a guide on how to search for travelogues from the project's corpus in the 
**online public access catalog** (OPAC) [*Quicksearch*](https://search.onb.ac.at/primo-explore/search?vid=ONB&lang=en_US) of the *Austrian National Library* (ONB) and on how to look at the digitized item in the ONB's viewer. In the result list of your Quicksearch query you find a link labeled **"Online access"** for every digitized item. Clicking on this link the viewer will open in a separate browser window. 

![Access digitized item in the ONB Viewer](/images/Fulltext-for-travelogue_Screenshot_1.jpg)

By right-clicking over any page (s. Screenshot), a menu opens up. You may rotate the image to the left or to the right. You may also download either the page currently shown ("Bild herunterladen") or the whole book ("Buch herunterladen").

![Download-menu in the ONB Viewer](/images/Fulltext-for-travelogue_Screenshot_2.jpg)

In the viewer application you can search for any string in the fulltext (e.g. "Pyramide). The results are marked in the text and you can click through the selected result pages in the menu bar (e.g. "Bild 1 von 7 mit Treffern"). 

![Search the fulltext in the ONB Viewer](/images/Fulltext-for-travelogue_Screenshot_3.JPG)

## How to get the fulltext for a travelogue ##

For downloading fulltext of a single travelogue (i.e. fulltext of one digitized copy) we offer a [Jupyter-Notebook](https://labs.onb.ac.at/gitlab/georgp/sacha-txt-downloader/) in the [*ONB Labs*](https://labs.onb.ac.at/en/) GitLab named "txt-downloader". By running this notebook, you will get a ZIP-folder in the output-repository of the Binder application, which you may download. The ZIP-folder contains plain-text-files for each page plus a text-file, in which all text-files of the single pages are combined into one file. Please note that neither structural metadata for page sequence is contained in the combined text file nor markeup for page breaks. 

>**Note:** Each digitized item is identified by a **barcode** (e.g. *Von der Alster zu den Pyramiden* +Z257607709). For downloading fulltext via the ONB Labs Jupyter Notebook you have to input the barcode identifier of the item, for which you want to download the fulltext. You can find the barcode in the item overview, which opens by clicking on a single result for your search query in the *Quicksearch* catalog. Please copy the barcode!

![Barcode for digitized item](/images/Fulltext-for-travelogue_Screenshot_6.jpg)

As soon as you have copied the barcode identifier for the digitized travelogue, you can start running the [Jupyter-Notebook](https://labs.onb.ac.at/gitlab/georgp/sacha-txt-downloader/). 

![Notebook in the ONB Labs GitLabs](/images/Fulltext-for-travelogue_Screenshot_4.JPG)

The first step is to click on **launch binder**. A Binder instance is being launched in a separate browser window. As soon as the Jupyter-notebook opens up you may start the application by clicking the ![run](/images/Fulltext-for-travelogue_Screenshot_5.JPG) button. By re-clicking the run button three times an input-bar appears. Please enter the barcode (see **Note** above) in the form of the example given and press return. 

![Enter barcode](/images/Fulltext-for-travelogue_Screenshor_7.jpg)

Proceed to the next "In" command, click on the command box and then click the ![run](/images/Fulltext-for-travelogue_Screenshot_5.JPG) button until the single text-files are being downloaded. At the end you will get a link to a ZIP-file ("barcode.zip"). 

>**Note**: **Only non commercial use** is allowed for images of ONB's digitized items as well as fulltexts. Please note the [right statement](https://rightsstatements.org/page/NoC-NC/1.0/?language=en) for items digitized in public-private-partnership with Google, as are all digitized travelogues of our corpus. 

For help or further information please contact our librarian at <martin.krickl@onb.ac.at>.

