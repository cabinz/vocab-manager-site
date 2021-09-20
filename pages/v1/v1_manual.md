---
title: User Manual v1.0.0 - v1.1.0
keywords: 
last_updated: 2021-9-20
summary: All the features and using details of Vocab Manager 1.x.
sidebar: v1_sidebar
permalink: v1_manual.html
folder: v1
---

## 1. Home Page

{% include image.html file="v1_manual/app-home.png" alt="" caption="" %}

After installation, a shortcut of Vocab Manager 1.x will be on your desktop. Double click it to open the software gettint into the home page.

There are two buttons on the homepage. Click the upper one, "Notebook", to get into the notebook page for vocabulary editting. The lower one, "Quiz", is for remembering test of the vocabulary added into the notebook.


## 2. Notebook

There are two available tables in notebook page, Word Editor table and Tag Editor table. You can shift back and forth using the table labels on the top of the table page.


### 2.1 Word Editor

Word Editor is horizontally split into two regions. The left one is Word List and the right one is the Detail Board.


#### 2.1.1 Word List

Word List mainly consists of the Search Box on the top and the List below. 

Initially, all the available words are displayed in the List. Using Search Box, you can filter the word you want, which will be on screen in real time. The number of filtered words will also be displayed below the Search Box. 

If you want to remove a word, select the word in the List and click "Remove" button at the bottom.

{% include image.html file="v1_manual/word-list-filter.png" alt="" caption="" %}


#### 2.1.2 Detail Board

Vocab Manager aims to serve as a highly customized vocabulary management tool, so that users from different fields (especially various professional fields) can use it as their specific requirements. Therefore, users are encouraged to input all the details of words, including spellings, definitions, contexts and notes. After pre-defining tags in the Tag Editor, users can also use them for tagging words.

* Spelling, definition, context, note are required manual input. Only the spelling of the word/phrase cannot be empty.
* If you pre-defined some tags in the Tag Editor table, they can be found in the drop down list of the Tagging Box. Select the one you want to tag on the word and click "Tagging" to add it.
* If you want to remove a tag from a word, select the tag in the list of the Tagging Box and press "Delete" on your keyboard.
* Double click a tag in the list to jump to the detail page of it in the Tag Editor table.

**All changes made in the Detail Board must be committed by clicking "Create" or "Update" below.**  "Create" button is for adding a new word in your notebook while "Update" button is for modifying the selected word in the Word List. Keyboard shortcut for "Create" is "Ctrl + Shift + Enter". And for "Update" there is "Ctrl + S".

The "Clear" button in the middle of the bottom will clean all the user input on the board, getting ready for inputs of a new word.

{% include note.html content="From v1.1.0 on, SHIFT in all keyboard shortcuts are removed, shortcut for \"Create\" become \"Ctrl + Enter\"" %}

{% include note.html content="From v1.1.0 on, word editor supports auto-filling the definitions and contexts (examples) of **English words** with contents crawled from Longman dictionary web page. The keyboard shortcut for auto-filling is \"Ctrl + F\": using in word spelling text box will automatically fill blank box(es); using in definition/context text box will append the content to the end of the current text. You can also find auto-filling options in the \"Auto Fill\" box of top menu, where \"Fill All\" is for auto-filling all records in the notebook." %}

{% include image.html file="v1_manual/word-detail-editor.png" alt="" caption="" %}



### 2.2 Tag Editor

The Tag Editor is also split into two parts like Word Editor, where the left part is Tag List and the right part is the Tag Detail. 

The controlling on Tag Editor is basically the same as that on Word Editor, meaning that every change will be saved only after committing by button clicking or shortcuts.

An extra part of Tag Editor is the Tagged Words Box, where all the words with currently selected tag in the Tag List are shown. Double clicking on the word in Tagged Word Box will bring you to the details of it in Word Editor table.

{% include image.html file="v1_manual/tag-viewer.png" alt="" caption="" %}



### 2.3 Tool Menu

The tool menu on the left top support two functions currently.

* "export as markdown" under "File" can export all your vocabulary as a markdown file, which user can convert into any format and print for reviewing on any devices.
* "Recycle Bin": All the removed word will be thrown into the recycle bin waiting for recovery or permanent deletion.

{% include image.html file="v1_manual/top-menu.png" alt="" caption="" %}



The markdown file exported is like: 

{% include image.html file="v1_manual/output-markdown.png" alt="" caption="" %}



## 3. Quiz

The Quiz window is a self-testing of vocabulary in the notebook. By showing the spellings of the words, users can press "Remember" or "Forget" to keep going.

All the test results will be recorded. The displaying order of the words is according to the history forgetting ratio.

{% include note.html content="From v1.1.0 on, the history statistical test information is displayed on the quiz form. And users can remove the momerized word into recycle bin directly during the quiz." %}

{% include image.html file="v1_manual/quiz-form.png" alt="" caption="" %}



### 3.1 Load Quiz

Currently, Vocab Manager supports loading all words for quiz or loading by tags.

{% include image.html file="v1_manual/load-quiz.png" alt="" caption="" %}

After loading the quiz, the buttons below will become activated.

{% include image.html file="v1_manual/start-quiz.png" alt="" caption="" %}



### 3.2 Remembering Test

If you remember the word displayed in the middle top of the window, click "Remember" to move forward.

{% include image.html file="v1_manual/remember.png" alt="" caption="" %}


If you forget the details about the word, just click "Forget" to check the infomation of the word.

{% include image.html file="v1_manual/forget.png" alt="" caption="" %}

Click "Next" for the next one after reviewing the details of a word.

{% include image.html file="v1_manual/detail-hint.png" alt="" caption="" %}



### 3.3 Test Report

When running out all the loaded words, "No more records" will be on screen. You can click "generate report" under "File" to export the test report of the Quiz, which contains all details of the words you forgot.

Actually, you can click to generate report at any time during the quiz and the report will cover only the forgotten words you've passed so far.

{% include image.html file="v1_manual/export-report.png" alt="" caption="" %}