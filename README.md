# Cyber Forensic Investigation Project
## Objective
This investigative project was conducted in late 2023. I was provided with three images, each from different devices—an iPad, an Android device, and a laptop. My objective was to scrutinize these images for potential threats. It was assumed that the perpetrator had incriminating evidence related to theft and plans to deface a museum within these images.

### Skills Learned
- Investigation
- Retreiving Evidence

### Tools Used
- Autopsy
- OSForensic
- SQLite database
- Windows Server 2016
- Kali Linux

## Methodlogy 
To ensure prevention of alterations, images (E01) were stored on a secured thumb drive and accessed via a freshly created virtual machine. Hashes were initially generated before examination to maintain consistency. Subsequently, the same thumb drive was used to preserve the evidence found.

Meticulous examinations of these pieces of evidence were carried out to capture any potential elements that could offer valuable insights for building the case. Other applications, such as Database SQLite, Google Maps, and Translation, were also employed to strengthen the case.

Below are the pieces of evidence found pertaining to two potential criminal cases: Defacement of a target in the National Gallery and a Stamp Heist. Additional supporting evidence can be found in the Appendices.

## Findings
- Finding One
  
We retrieved deleted Gallery documents related to the Security Schedule from Carry's tablet using OSForensic's Deleted File Search. When compared with Tracy's copy found on Tracy’s own external device, it became evident that the documents were identical. The parts determining the similarities were the Gallery’s name, logos, and the title ‘Security Personnel Schedule’.

Metadata revealed that Carry's document was created with a timestamp of '12/07/12, 3:15 PM,' while Tracy accessed the document at '12/07/12, 7:53 AM,' potentially suggesting Tracy had accessed it first and shared the document with Carry afterward.

![Screenshot 2024-04-17 115346](https://github.com/JolynNgSC/Cyber_Forensics-/assets/164031233/f51f772f-9939-4e53-9808-7014df39d413)

- Finding Two
  
Carry's tablet contained unallocated space that held conversations between Carry and Alex. A link to a video was shared between them, and Carry had downloaded the video, which was later viewed by the investigator.

The initial start of the video showed two hands with lipstick and eyes. Gibberish was spoken, followed by a fade transition before the imagery turned into a sequence of photos with a male AI voiceover, identified as Alex.

The first image showcased the intended target for defacement. Subsequently, the second image featured four men, indicating that these individuals were associates of Alex. Other email interactions were uncovered, signifying that Carry had watched the video and agreed to assist Alex. These emails pertained to the preparation of digital signatures for the associates.

![Screenshot 2024-04-17 115539](https://github.com/JolynNgSC/Cyber_Forensics-/assets/164031233/b5adae5a-5f96-42d7-9938-a91ac6163b70)![Screenshot 2024-04-17 115551](https://github.com/JolynNgSC/Cyber_Forensics-/assets/164031233/4fd056e7-8cfa-40c7-baed-851648c7de2e)

- Finding Three
  
The physical presence of Carry and Tracy in various locations was identified through examination of Carry’s tablet and Tracy’s phone. Specific images containing text were identified to provide insights into their specific location.

The timestamps of the locations were then confirmed using Autopsy. Carry was found to be physically present at Fairfax, Arlington, Bethesda Bagels, and Virginia Avenue on timestamp '09/07/12,' throughout the day. This was in the order determined by the timestamps, which was four days after Alex's first correspondence.

Google Maps searches were used to examine these mentioned locations. The findings revealed that Fairfax and Arlington are located outside of Washington, D.C., while Virginia Avenue and Bethesda Bagels are within the city. The trip between Bethesda Bagels and Virginia Avenue takes approximately 10 minutes, which nearly aligned with the metadata they possessed—12 minutes.

Notably, during this journey, Carry would have driven past The National Gallery. On the other hand, Tracy's physical whereabouts don't seem to align directly with Carry's, as there were no pictures indicating they were together physically, and Tracy's photos were taken a day before Carry's.

![Screenshot 2024-04-17 115748](https://github.com/JolynNgSC/Cyber_Forensics-/assets/164031233/4b6c4f86-7b4d-49ee-a0ae-13e478210ad0)

- Finding Four

Evidence from email conversations discovered through Carry’s tablet database indicated that Carry came into contact with Tracy on '05/07/12' through Facebook. It was also observed that more exchanges contained mentions of ‘events’ and ‘security schedule’. On timestamp '12/07/12', email exchanges stating that Carry had added Tracy and Alex on Google+ were found through autopsy in plain text.

- Finding Five

The investigator extracted a password-protected zip folder from Tracy's phone through Autopsy and employed OSForensic to conduct a password search, successfully unlocking the folder with the password 'Hercules.' Within the folder, a series of PDF files outlined damage fees for various stamps. It was also noted that these damage fees did not include transport fees. Several pictures of the stated stamps were also found using OSForensic Deleted File Search.

Emails between Tracy, Pat, Perry, Carol, and King were also uncovered, and the conversations revealed some of the named personnel's money and parole issues, which likely indicated intent for the Stamp Heist.

Lastly, a text file named 'needs.txt' under the extension mismatch category was uncovered through Autopsy via Tracy’s phone. It indicated a list of materials needed for a possible Flash Mob or Stamp Heist.

