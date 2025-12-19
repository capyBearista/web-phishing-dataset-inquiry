# Exploration of Website Phishing Dataset

## Objective of this Repository
This repository is dedicated to the exploration and analysis of the Website Phishing dataset sourced from the UC Irvine Machine Learning Repository. The primary objectives include:
- Understanding the structure and features of a dataset.
- Performing exploratory data analysis (EDA) to uncover patterns and insights.
- Preparing the data for potential machine learning applications in phishing detection.

## Dataset

[Website Phishing](https://archive.ics.uci.edu/dataset/379/website+phishing) from UC Irvine Machine Learning Repository
- Created by [Phishing detection based Associative Classification data mining](https://www.semanticscholar.org/paper/Phishing-detection-based-Associative-Classification-Abdelhamid-Ayesh/867e2293e9780b729705b4ba48d6b11e3778e999) (Abdelhamid et al., 2014)

### Description
*(Provided by repository)*

> The phishing problem is considered a vital issue in the e-commerce industry especially e-banking and e-commerce taking the number of online transactions involving payments.
> 
> We have identified different features related to legitimate and phishy websites and collected 1353 different websites from difference sources. Phishing websites were collected from Phishtank data archive (www.phishtank.com), which is a free community site where users can submit, verify, track and share phishing data. The legitimate websites were collected from Yahoo and starting point directories using a web script developed in PHP. The PHP script was plugged with a browser and we collected 548 legitimate websites out of 1353 websites. There is 702 phishing URLs, and 103 suspicious URLs.
> 
> When a website is considered SUSPICIOUS that means it can be either phishy or legitimate, meaning the website held some legit and phishy features.

### Variables Table

| Variable Name      | Role    | Type    | Description |
|--------------------|---------|---------|-------------|
| SFH                | Feature | Integer | Whether the form handler is on the same domain
| popUpWindow        | Feature | Integer | Presence of pop-up windows that ask for personal information
| SSLfinal_State     | Feature | Integer | SSL certificate status and validity
| Request_URL        | Feature | Integer | Percentage of external objects in the page
| URL_of_Anchor      | Feature | Integer | Percentage of anchor URLs pointing to different domains
| web_traffic        | Feature | Integer | Website traffic rank from Alexa
| URL_Length         | Feature | Integer | Length of the URL
| age_of_domain      | Feature | Integer | Age of the domain registration
| having_IP_Address  | Feature | Integer | Whether URL uses IP address instead of domain name
| Result             | Target  | Integer | Website Phishy-ness classification

**Possible Values**
- Features: 1 = Phishy, 0 = Suspicious, -1 = Legitimate (mostly)
- Target: -1 = Phishy, 0 = Suspicious, 1 = Legitimate

No missing values present.

### Sources of Data

- Phishing Websites: The researchers sourced 752 phishing sites from PhishTank and Millersmiles. These platforms are community-driven archives where users report and share data on known phishing attacks.   
- Legitimate Websites: They collected 601 legitimate sites from the Yahoo Directory.  

**Collection Methodology**: To gather this data efficiently, the authors developed a specific web script written in PHP. This script was embedded directly into a web browser, allowing them to automatically browse, scrape, and extract the necessary feature data from the 1,353 total websites included in the study.