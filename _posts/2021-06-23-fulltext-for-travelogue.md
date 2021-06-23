| title | share | permalink |
| ----  | ----  | ---- |
| Fulltext for travelogue | true | /2021-06-23-fulltext-for-travelogue |

#### Searching for Travelogues ####

In our post [Searching for Travelogues](https://travelogues-project.info/2021-04-21-searching-for-travelogues/) we have offered you a guide on how to search for travelogues from the project's corpus in the 
**online public access catalog** (OPAC) [*Quicksearch*](https://search.onb.ac.at/primo-explore/search?vid=ONB&lang=en_US) of the *Austrian National Library* (ONB). 

In this blog post we have also described how you may look at the digitized item in the ONB's viewer. In the result list you find a link labeled **Online access** for every digitized item. Clicking on this link the viewer will open in a separate browser window. By right-clicking over any page (s. Screenshot), a menu opens up. You may rotate the image to the left or to the right. You may also download either the page currently shown ("Bild herunterladen") or the whole book ("Buch herunterladen").

![Download-menu in the ONB viewer](/images/Fulltext-for-travelogue_Screenshot_2.jpg)

In the viewer application you can search for any string in the fulltext (e.g. "Pyramide). The results are marked in the text and you can click through the selected result pages in the menu bar. 

![Search the fulltext in the ONB Viewer](/images/Fulltext-for-travelogue_Screenshor_3.jpg)

#### How do I get the fulltext for a travelogue? ####

For downloading fulltext of a single travelogue (i.e. fulltext of one digitized copy) we offer a [Jupyter-Notebook](https://labs.onb.ac.at/gitlab/georgp/sacha-txt-downloader/) in the [*ONB Labs*](https://labs.onb.ac.at/en/) GitLab named "txt-downloader". By running this notebook, you will get a ZIP-folder in the output-repository of the Binder application, which you may download. The ZIP-folder contains plain-text-files for each page plus a text-file, in which all text-files of the single pages are combined into one file. Please note that neither structural metadata for page sequence is contained in the combined text file nor markedup for page breaks. 

>**Note:** Each digitized item is identified by a **barcode** (e.g. *Von der Alster zu den Pyramiden* +Z257607709). For downloading fulltext via the ONB Labs Juypter Notebook you have to input the barcode identifier of the item, for which you want to download the fulltext. You can find the barcode in the item overview, which opens by clicking on a single result for your search query.

![Barcode for digitized item](/images/Fulltext-for-travelogue_Screenshot_5.jpg)

![Notebook in the ONB Labs GitLabs](/images/Fulltext-for-travelogue_Screenshot_4.jpg)

By clicking on **launch binder** a Binder instance is being launched. As soon as the Jupyter-notebook opens up you may start the application by clicking the ![run](/images/Fulltext-for-travelogue_Screenshot_5.jpg) button. By re-clicking the run button three times an input-bar appears. Please enter the barcode (see **Note** above) in the form of the example given.  

