DESCRIPTION:
XML downloader for SciTech Connect XML Services. 
Downloads metadata XML for all found search results, 
taking in account multiple pages with search results.
Extracts SciTech links and OSTI identifiers from XML files. 

INSTRUCTIONS:
First ind the search qurery which equals the following <link> by following this manual: 
http://www.osti.gov/home/sites/www.osti.gov.home/files/SciTechXMLDataServices.pdf
and download XML files into a folder with download_xml_services.py. 
To obtain a text file with all links out of the downloaded files, use the 
--identifier_links option. The links are saved in a subfolder
with the respective option name in individual files for each XML file 
and as a collected file with all identifiers or links extracted out of
a folder.

USAGE:
Locate file in Terminal and type:
1) python download_xmls_services.py --download <link> <ResultFolder>
2) python download_xmls_services.py --option <XMLFolder>
options are --identifier_links, --identifiers, --links

EXAMPLE:
python download_xmls_services.py --download http://www.osti.gov/scitech/scitechxml?searchFor=batter* batter
python download_xmls_services.py --identifier_links batter

AUTHOR:
Simon Engelke (engelke.co)

LICENSE:
MIT

VERSION:
1.0

More details in the individual Python files.

This code was developed as part of [Google Summer of Code 2014](https://www.google-melange.com/gsoc/project/details/google/gsoc2014/sengelke/5668600916475904)