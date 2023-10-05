## Contributing Guidelines

Welcome to the Sinhala Annotated Corpus repository! We are excited to have you contribute to our project. This repository is only for Sinhalese in Sri Lanka or anyone who have much undrstanding on Sinhala Language. Let's make your contribution to open source and earn a Hacktoberfest badge.

If you are new to contributing to open source, please read the following resources:

* [How to Contribute to Open Source](https://www.freecodecamp.org/news/how-to-contribute-to-open-source-projects-beginners-guide/)
* [GitHub Guides](https://github.com/git-guides)

## About this Repository

The purpose of this repository is create a Sinhla News Article Corpus. This repo can be used by anyone how work with NLP and NER tasks related to the Sinhala NLP tasks. Currenty this annotated corpus collection is used for the ongoing research that **'Sinhala Document Clustering using Name Entity Recognition'** 

## How to contribute for this repo

1. Star the repository.
2. Fork the repository.
3. Make your changes.
4. Submit a pull request.

## Star the repository

Click on the **Star** button in the top right corner. Make sure that repository **starred**.

## Forking the repository

To fork the repository, click on the Fork button on the repository's GitHub page. This will create a copy of the repository in your own GitHub account.

- **Clone** your fork down to your local machine

```markdown
git clone https://github.com/DininduChamikara/SAC_Hacktoberfest2023.git
```

- Create a branch

```markdown
git checkout -b branch-name
```

## Making your changes

Once you have forked the repository, make your changes to the code. Be sure to follow the coding style guidelines for the programming language that you are contributing to.

Here the example for how to do changes

Available Code in the repo is like below.

```markdown
    [
      "පරිසර හිතකාමී ප්‍රවාහන මාධ්‍ය සඳහා නෙදර්ලන්තය විශාල ප්‍රසිද්ධියක් උසුලනවා. “Bakfiets” පා පැදි යනු ඉන් එකක් පමණ යි.",
      {
        "entities": [
          ["පරිසර", 0, 5, ""],
          ["හිතකාමී", 6, 13, ""],
          ["ප්‍රවාහන", 14, 22, ""],
          ["මාධ්‍ය", 23, 29, ""],
          ["සඳහා", 30, 34, ""],
          ["නෙදර්ලන්තය", 35, 45, ""],
          ["විශාල", 46, 51, ""],
          ["ප්‍රසිද්ධියක්", 52, 65, ""],
          ["උසුලනවා.", 66, 74, ""],
          ["“Bakfiets”", 75, 85, ""],
          ["පා", 86, 88, ""],
          ["පැදි", 89, 93, ""],
          ["යනු", 94, 97, ""],
          ["ඉන්", 98, 101, ""],
          ["එකක්", 102, 106, ""],
          ["පමණ", 107, 110, ""],
          ["යි.", 111, 114, ""]
        ]
      }
    ],
```
Your task is to identify the named entities on each word. The applicable named entities are only ["LOCATION", "PERSON", "ORGANIZATION", "DATE", "TIME"]. If any word not related to any of this Named Entities just simply remove it.

Each entity array include the [word, starting index, ending index, Named Entity].

After identifying the named entity Just add the named intity class as final string of the array and simply remove the word string from the array. 

The final output is like below.

```markdown
    [
    "පරිසර හිතකාමී ප්‍රවාහන මාධ්‍ය සඳහා නෙදර්ලන්තය විශාල ප්‍රසිද්ධියක් උසුලනවා. “Bakfiets” පා පැදි යනු ඉන් එකක් පමණ යි.",
        {
            "entities": [
                ["නෙදර්ලන්තය", 35, 45, "LOCATION"],
            ]
        }
    ],
```
For one pull request it is enough to change one object from the corpus.

Make sure to refer previes examples and correctly identify the named entities. 

-----------------------

After that just Commit and push your chages using below commands.

```markdown
git add .
git commit -m 'Commit message'
git push origin branch-name
```

## Submitting a pull request

Once you have made your changes, submit a pull request to the original repository. Be sure to include a clear and concise description of your changes in the pull request.

- Create a new pull request from your forked repository (Click the `New Pull Request` button located at the top of your repo)
- Wait for your PR review and merge approval!
- [Follow me](https://github.com/DininduChamikara) for getting fast PR approvels. 

## Additional guidelines

* Please re-check your changes thoroughly before submitting a pull request.
* Be respectful of other contributors and the project maintainers.

## Thank you for your contributions!

We appreciate your help in making this repository a valuable resource for the programming community and the Sinhala NLP developing community.

## Code of Conduct

This repository follows the [Contributor Covenant](https://www.contributor-covenant.org/) code of conduct. Please be respectful of other contributors and follow the code of conduct at all times.
