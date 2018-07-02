# Challenges of Export/Import using the MedBiquitous Virtual Patient ANSI/MEDBIQ VP.10.1-2010 standard - FAQ

## What is the MedBiquitous Virtual Patient ANSI/MEDBIQ VP.10.1-2010 standard?
The [MedBiquitous Virtual Patient ANSI/MEDBIQ VP.10.1-2010 standard](https://medbiq.org/medbiquitous_virtual_patient) was developed by [MedBiquitous](https://medbiq.org), a consortium that develops health professions technology standards. The Virtual Patient (VP) standard defines an XML schema for describing VP resources which allows VP resources to be exported and imported into standard-compliant systems. The standard builds upon the existing [Healthcare Learning Object Metadata](https://hmedbiq.org/healthcare_learning_object_metadata) and [SCORM 2004 4th Edition](http://www.adlnet.gov/research/scorm/scorm-2004-4th-edition/) standards.

Effective VPs are widely recognised to be difficult to create, so the goal of the standard is to enable the exchange of these resources between individuals and systems, allowing wider access to examples of these resources, and to allow educators to share and repurpose resources for their learners. The standard (sometimes known as Medbiq VP or even MVP) was used by the EC-funded [eViP](http://virtualpatients.eu) program to facilitate the development of a shared bank of 340 VPs, and that project contributed to the development of the standard.

## Why do the Virtual Scenarios in the WAVES project use a standard called Virtual Patients?
Simply because, in most cases, there is no difference between the two! A Virtual Patient (VP) is simply a Virtual Scenario (VS) that has a setting in a healthcare context. Most VS can be represented using the VP standard.

The primary reason why the standard is designed for VPs is that those who developed it were working in medicine and healthcare education, so they chose to use the word "patient". However, it soon became apparent that this technology can be used for more than just healthcare. There are some healthcare-specific elements in the VP standard, but they can simply be omitted when a scenario does not need to use them.

## What VS systems support the standard?
There is no definitive list of the systems that support the standard. However, the systems used in the WAVES project, [Casus](https://www.instruct.eu/en/) and [OpenLabyrinth/OLab](http://openlabyrinth.ca), do support the standard.

## What can the standard do?
The standard allows standards-compliant VS systems to export the cases as content packages in the form of a zip file that is structured so as to adhere to the standardised specification. This means that another standards-compliant VS system can read and import the file and will know where it can retrieve the relevant information from the content package.

As a result, the standard means that you can take a case from one system, and move it to another system. These systems can be different installations of the same system (i.e. if you are moving a VS from one installation of OpenLabyrinth to another) or different systems (i.e. moving a VS for OpenLabyrinth to Casus). You could even use the standard to export and import a VS back into the original system, thus creating a duplicate case that you can edit.

## What can't the standard do?
The standard is not a VS "player", and VS files stored using the standard cannot simply be double-clicked, opened on any machine and used to play a scenario. Instead, you need an installation of a standards-compliant VS system, such as OpenLabyrinth or Casus, into which you can import your VS.

By necessity, the standard offers a generic description of a VS resource; that is, it's designed to be a general solution that can apply to all the many different types of VS. However, all the different VS systems offer differing functionality, with a complex range of advanced features. Unfortunately, this means that not all aspects of a VS in a particular system can necessarily be stored within the standard.

As an analogy, it is best to consider the VS standard to be a "lossy" data format, much like a jpeg image. When storing an image as a jpeg, you sacrifice some of the fine detail from the raw image file in order that the file be smaller in size, quicker to load, and more universally readable. The same sacrifice is made when the VS standard is used; some of the system-specific features of a VS case, which will not be usable in another system, will be lost as a result of using the standard as a trade-off to allow the basic fundamentals of the VS to be imported into another system.

If you wish to export a VS and all its advanced features so that you can import it into another instance of the same system, then many systems will offer their own, non-standardised data formats that you can use to achieve this. These formats are unlikely to be able to be recognised by other, different VS systems.

## What aspects of a VS does the standard include?
The structure of the standard, and how it describes a VS in technical detail is beyond the scope of this document. The files and schema which make up the standard can be found in full on  [the MedBiq VP GitHub page](https://github.com/medbiq/medbiq/tree/master/virtualpatientdata/v1). The exact elements of a VS supported will vary from system to system, so you should consult the documentation for your system.

However, in general the standard can include the text-based content and media files, any decision-making or branched options, and any metadata. It may include any MCQs or questions, and mechanisms for scoring or updating values such as blood pressure or heart rate throughout the VS. If your case is created using a visual editor, the standard may also include some details of the layout of your case map.

## Where can I find examples of the standard?
You can find examples of VS cases to play on the web on the [WAVES website](http://www.wavesnetwork.eu/index.php?pg=toolkit--d-3-2-exemplar-scenarios), many of which will also included downloadable content packages that use the standard. Similarly, there are a lot of VS cases freely available to download from the [eVip programme](http://virtualpatients.eu/referatory) website. All these VS are made available under [Creative Commons](http://www.creativecommons.org) licences that allow them to be freely used and shared subject to the specific conditions of that licence.
      
## How can I use the standard to play a Virtual Scenario?
You will need to have access to a VS system, such as OpenLabyrinth or Casus. In most systems, when you are logged into them with "Author" permissions you will find an option in the system interface to import a scenario using the "Medbiq VP" standard. Select the content that you wish to import, and follow the instructions provided by the system. An imported case can then be played in the same way as any other case.

Please note that you cannot play a case directly from the standardised file.

## What can I expect when I import a VS?
When you import a VS case into a system, you should not expect it to be fully playable and completely organised in the new system immediately. Some of the system-specific features of a VS case may have been lost as a result of using the standard, and different systems may interpret the standard slightly differently. This is true of all technology standards; imagine the situation when you open a web page in different browsers and they each work slightly differently. Alhough the web page is standardised (using the HTML standard) each of Chrome, Firefox, Safari and Internet Explorer are required to interpret the information, and will likely do so differently. The standard does however ensure that the fundamentals of the information provided remain intact and readable.

When you first import a VS you should try to play it, first to see if it works at all, and then to identify if there are any modifications that need to be made in order for it to make sense in its new setting. These modifications can be made using the authoring tools of the system to which the case was imported, and may include relinking some media files, resetting the starting point of a case, or changing aspects of the scenario to account for any features that are no longer present in the new system.

The number of changes needed post-import will depend upon the similarity of the importing and exporting system. If the two systems are the same, then you can expect to have relatively few changes required. However, if the two systems are very different in nature, there may be more work involved in adapting the scenario in the new system so that it is logical and coherent to the learner.
