# Fishikawa Project
The **Fishikawa Project** and the Fishikawa - **Problem Determination Aide** (PDA) json database are a community based, open Source project aimed at providing access to problem diagnosis and resolution information regarding common issues or problems that may be observed when installing, running or managing the Joomla!® Open Source CMS, with the view to reducing barriers to entry, early stage frustrations and improving end-user satisfaction and long-term preferential choice of Joomla!

**Problem Determination Aide**  
The PDA is a structured data "_json_" database made available for download or inclusion in 3rd Party scripts, applications or Joomla! extensions. The database contains a growing number of common and well known server, php and Joomla! misconfigurations or issues that may cause problems for site administrators and/or end-users.
  
  
---
  
  
#### The _PDA json database_ structure is defined as;  
- **\[dataset\]**
  - **version** - Version (_x.y.z_) 
  - **package** - Joomla!
  - **subpackage** - Fishikawa
  - **category** - Problem Determination Aide 
  - **license** - GNU GPLv3 or later license
  - **copyright** - Fishikawa Project 2020, @RussW, @mandville, @frostmakk
  - **link** - https://github.com/FishikawaRCA/pda
- **\[pdc/key\]** - Problem Determination Code, four (4) character code  
  _refer detailed information below..._
  
  
**Each individual _\[pdc\]\[key\] record_** contains the following structured elements;  
- **\[pdc\/key\]** - Problem Determination Code  
  a four(4) character code, _\[_ _0-F_, _0-F_, _0-F_, _0-F_ _\] (eg: 01A5)_
  - **heading** - a short, 82 characters or less
  - **description** - a more detail problem description
  - **category** - _a single word or hyphenated phrase describing the most likely effected resource area_  
    _eg: php, security, installation_
  - **severity** - how severely this problem effects the operation of Joomla
  - **symptoms** - _up to four (4) items describing the most likely observed symptom_
  - **causes** - _up to four (4) items describing the most likely causes_  
  - **effects** - _up to four (4) items describing the most likely effected individual resources or activities_
  - **actions** - _up to four (4) items describing the most likely actions to resolve this problem_

> _**3PD Note:**_  
_Whilst designed with "**universal use**" in mind, the PDA database has origonally been designed for, and is used by, the [Fishikawa - Root Cause Analysis companion project](https://github.com/FishikawaRCA/frca), therefore the following "_**Problem Codes**_" _(PDC)_ in this project repository are specific to, and relevant for, internal use by the FRCA script and may not serve your use-case;_
> - **0000** : Generic/Unknown/Unclassifed Error  
> - **0001** - **0049** : are used by FRCA script internally
  
  
---
  
    
## Problem Determination Aide Entry Contributions
Contributions to _**this json database repository**_ are more than wlecome, but need to conform to the following element specifications;

- **heading** (short) : **82** charcters or less
  
- **severity** :
  - **1** - Fatal/ShowStopper/High  
  - **2** - Partially Unuseable/Medium  
  - **3** - Non-Fatal/Recoverable/Low
  - **4** - Reference/Notice/Unclassifed

- **symptoms, causes, effects & actions**
  - may contain **limited html** \<p\>, \<b\>, \<strong\>, \<i\> _(FRCA will strip all other html)_ and preferably under 200 characters in length
  
  
---
  
  
### Security Policy
The PDA json database is provided publicly, _**as-is**_, in itself a json database _**is not intrinsically insecure**_, **how you access and use it might be though**, it is _**your responsibility**_ to ensure you understand the implcations and intricacies of including remote files in any 3PD application before use.
  
  
---  
  
  
## Contributing - _Get Involved..._

### Language Translations
If you would like to contribute or help with translating the PDA, please visit the [PDA-Translations repository](https://github.com/FishikawaRCA/pda-translations) for more information.
  
  
## Other Fishikawa Project Initiatives
The PDA database is extensively used by the Fishikawa "_**Root Cause Analysis**_" _(FRCA)_ project, to find out more about this project, please visit the [Fishikawa FRCA repository](https://github.com/FishikawaRCA/frca).  
  
  
---
  
  
##### Licensing & Notices
> **The PDA comes with ABSOLUTELY NO WARRANTY.** _This is free software, and covered under the GNU GPLv3 or later license. You are welcome to redistribute it under certain conditions._
>
> _For details read the LICENSE file included in the download package with this script. A copy of the license may also be obtained at https://www.gnu.org/licenses/_

> _**The Fishikawa Project & PDA json database** are not affiliated with or endorsed by The Joomla! Project™. Use of the Joomla!® name, symbol, logo, and related trademarks is licensed by Open Source Matters, Inc._
