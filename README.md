# Intro to Android Grading Guide

## Table of Contents
- [General Grading Instructions](#general-grading-instructions)
- [A2](#a2)
- [A3](#a3)
- [A4](#a4)
- [A5](#a5)
- [A6](#a6)

## General Grading Instructions
1. Download and extract your students' zip files.
2. Open their projects in android studio.
3. Run their app and grade by the provided rubric! (Download as .txt, one for each grade.) (You mostly just have to test; should not need to look at code much at all)
4. Add their grade and attach the .txt to their CMS upload and submit!

## A2

### Notes
- Some students do not know to change `MainActivity.kt` to make their app show the real screen content. If this is the case, they likely just have a `@Preview` function for the `MainScreen()` you can run instead (and there's a -1 deduction for this).
- Make sure the timestamps on each expense row is unique (for the seconds portion) and not just showing the same timestamp.
- Test + and - quantity values! + should be green, - should be red.
- Don't worry about specifics of `.dp` and padding and stuff. That's not important.
- Watch the attached video for what the A2 soln should look like!

### Demo Video

https://github.com/user-attachments/assets/5bb46749-ebce-4548-bfd4-5a0f83d107e9

### Rubric

Rubric file: [A2 Rubric.txt](./A2%20Rubric.txt)

```text
Grader: <TODO Your Name>, <TODO Your NetID>


Total:             +12
Deductions:   -TODO
—----------------
Final Score:        TODO


[Remember to fill out the A2 feedback form for the final +1 pt!]


——————


Comments:


<TODO: Add encouraging comments here! Point out some nice things about their implementation, and give constructive feedback in a few places if possible.>


——————


Deductions:


<TODO: Apply the correct deductions, then DELETE THIS TEXT>


General
* [-6] App does not compile nor launch, even if the grader attempted to fix any local Gradle issues.
* [-1] Implementation not separated into different files. Each of ExpenseRow.kt, ExpenseHeader.kt, and MainScreen.kt should be implemented in their own files.


ExpenseRow.kt (3pts)
* [-3] Missing.
* [-1] Missing Title text. 
* [-1] Missing Date text.
* [-1] Missing Amount text.
* [-1] Amount text exists, but is not colored green if positive, red if negative. (OR) is not bolded.


ExpenseHeader.kt (4pts)
* [-4] Missing.
* [-1] Missing the Expense Name TextField.
* [-1] Missing the Expense Cost TextField.
* [-2/-1] Cannot type into text field(s).
* [-1] Missing title text.
* [-1] Missing button.
* [-2] No onClick functionality implemented.
* [-0.5] Previous text still persists even after onClick is fired. 
* [-0.5] Missing placeholder texts in one of the text fields.


MainScreen.kt (5pts)
* [-5] Missing.
* [-2] No LazyColumn used in implementation.
* [-1] Screen content not shown in real app launch (only in @Preview functions).
* [-1] System time of each grocery entry creation not shown in any way. (flexible deduction).
```

## A3

### Notes
- If an animation looks almost right, just give them full credit, and leave a comment. But if it's the wrong type of animation (i.e. using a `animateFloat` vs. `AnimatedContent`), deduct as appropriate.
- We don't expect anyone to have trouble not launching their app actually through `MainActivity.kt` this time around.

### Demo Video

https://github.com/user-attachments/assets/c182db25-001c-4a69-9b89-d06facb49d3f


### Rubric

Rubric file: [A3 Rubric.txt](./A3%20Rubric.txt)

```text
Grader: <TODO Your Name>, <TODO Your NetID>


Total:             +12
Deductions:   -TODO
—----------------
Final Score:        TODO


[Remember to fill out the A3 feedback form for the final +1 pt!]


——————


Comments:


<TODO: Add encouraging comments here! Point out some nice things about their implementation, and give constructive feedback in a few places if possible.>


——————


Deductions:


<TODO: Apply the correct deductions, then DELETE THIS TEXT>


General
* [-6] App does not compile nor launch, even if the grader attempted to fix any local Gradle issues.
* [-1] Implementation not separated into different files. Each of WalletRow.kt, TickerRow.kt, and StockDetailScreen.kt should be three separate files.


WalletRow.kt (3pts)
* [-1] (-1 per offense) Missing one of the texts: “Your Wallet,” the balance, or the percentage
* [-1] AnimatedContent does not swap out the percentage text whenever a stock is bought.
* [-1] Text is not green/red when positive or negative.
* [-1] WalletRow() not called on MainScreen()
* [-1] Balance displayed is not accurate


TickerRow.kt (4pts)
* [-1] (-1 per offense) Missing a UI element: stock title, stock balance, stock percentage
* [-1] Neither the percentage NOR the balance text animates out whenever the stock price changes
* [-1] Balance or percentage displayed is not accurate
* [-1] Text is not green/red when positive or negative
* [-2] Tapping does not navigate to the stock detail screen
* [-2] Missing from MainScreen()
* [-1] Does not show all the available tickers in the app (APPL, MSFT, GOOG, etc.)


StockDetailScreen.kt (5pts)
* [-1] (-1 per offense) Missing a UI element: stock title, stock price, stock percentage, wallet row, amount owned, buy/sell buttons
* [-2] Balance or percentage texts do not animate whatsoever.
* [-1] Balance or percentage texts simply use an AnimatedContent transition instead of an animateFloatAsState transition.
* [-2] Screen color does not change whatsoever.
* [-1] Screen color does not change smoothly (changes instantly).
* [-1] Pressing buy/sell a stock does not do anything.
* [-1] Information about the SPECIFIC stock pressed on the TickerRow is not shown/given to the screen.
```

## A4

### Notes
- This is a pretty easy assignment to grade--it's split into 5 parts that you can test just by running their app and looking in just one/two files.
- The minimum grade someone is able to get for submitting from now on is 6pts (half credit). If they get more deductions than that, just still grade them for 6pts.
- Make sure to look in the code that the students used the intended ViewModel logic to implement certain features, since there are ways to implement it without using MVVM (but this is reflected just in the deductions in the assignment, so just follow that.)

### Demo Video

https://github.com/user-attachments/assets/ba193c50-ce6f-4360-98af-2fc1bc98eb28


### Rubric

Rubric file: [A4 Rubric.txt](./A4%20Rubric.txt)

```text
Grader: <TODO Your Name>, <TODO Your NetID>


Total:             +12
Deductions:   -TODO
—----------------
Final Score:        TODO


[Remember to fill out the A4 feedback form for the final +1 pt!]


——————


Comments:


<TODO: Add encouraging comments here! Point out some nice things about their implementation, and give constructive feedback in a few places if possible.>


——————


Deductions:


<TODO: Apply the correct deductions, then DELETE THIS TEXT>


General
* [-6] App does not compile nor launch, even if the grader attempted to fix any local Gradle issues.


Reading the Message Flow (2pts)
* [-1] chatRepository not injected into the ChatViewModel
* [-2] Messages not showing up correctly (”Hello! Am I alone here?”)


Typing into the Text Field (3pts)
* [-3] Cannot type into the text field.
* [-1] Text Field implemented simply using a mutableStateOf() instead of using ViewModel up/down logic.


Sending a Message (2pts)
* [-2] Cannot send messages.
* [-1] isSendEnabled not used to incur send message button enabling/disabling.
* [-1] Typed message not cleared after send.
* [-1] chatRepository’s .sendMessage() is not used.


Reading the Header Flow Information (3pts)
* [-2] The name does not change from ??? to your typed-in philosopher’s name after you give the philosopher a name (by chatting with it)
* [-1] Inaccurate timestamp.
* [-1] Name not implemented using a .collect on botNameFlow.
* [-1] Timestamp not implemented using a .collect on timestampFlow.


Reading the Currently Typing Flow (2pts)
* [-2] A “...” does not pop up while the bot is typing.
* [-1] Not implemented using a .collect on currentlyTypingFlow.
```

## A5

### Notes
- none

### Demo Video

https://github.com/user-attachments/assets/52e65a5a-5d1a-4024-bdf8-d771adc0c75c


### Rubric

Rubric file: [A5 Rubric.txt](./A5%20Rubric.txt)

```text
Grader: <TODO Your Name>, <TODO Your NetID>


Total:             +12
Deductions:   -TODO
—----------------
Final Score:        TODO


[Remember to fill out the A5 feedback form for the final +1 pt!]


——————


Comments:


<TODO: Add encouraging comments here! Point out some nice things about their implementation, and give constructive feedback in a few places if possible.>


——————


Deductions:


<TODO: Apply the correct deductions, then DELETE THIS TEXT>


General
* [-6] App does not compile nor launch, even if the grader attempted to fix any local Gradle issues.


Network & Data Layer Setup (5pt)
* [-1] Missing necessary fields, incorrect data types, missing/incorrect @Serializable or @SerializedName annotations for Kotlin serialization in Product.kt
* [-1] Missing/incorrect @GET annotations, wrong paths/endpoints, missing/incorrect @Query for search, incorrect return types in ProductApiService.kt
* [-1] OkHttpClient Provider: missing or incomplete
* [-1] Retrofit Provider: Incorrect base URL, missing necessary converters (e.g., JSON).
* [-1] API Service instance not provided in the NetworkModule and/or not injected into the ProductRepository.


Repository & ViewModel Logic (4pt)
* [-1] ProductRepository: getAllProducts: Correctly calls API, uses Result<T> wrapper (or equivalent) for return type.
* [-1] ProductRepository: searchProducts: Correctly calls API with query parameter, uses Result<T> wrapper.
* [-0.5] ViewModel: Repository not injected or Any is not replaced with Product in UiState
* [-0.5] ViewModel: loadProducts and/or searchProducts not launched in viewModelScope
* [-0.5] ViewModel: In loadProducts and/or searchProducts, isLoading is not set to true before calling repository function and/or not set to false when the result is obtained
* [-0.5] ViewModel: In loadProducts and/or searchProducts, the products uiState field is not updated correctly


UI Integration (3pt)
[-1] Not collecting uiState and searchQuery from ViewModel
[-1] Not using LazyColumn and ProductCard correctly to display products
[-1] Not calling ProductScreenContent in ProductScreen or not passing in the parameters correctly
```

## A6

### Notes
- Grading A6 takes a blend of testing and looking at code: `HomeScreen`, `HomeViewModel`, `RatingScreen`, and `RatingViewModel`, although most of it is testing.
- Please take a look at the demo solution video to see how the app should behave first! The expected behavior is a bit unclear from the rubric, and students seem to be having trouble meeting the expectations.
- For the deduction: `* [-1] User does not automatically navigate 1 second after uploading a new image`. When you UPLOAD an image, 1 second later, you are supposed to automatically navigate to the rating screen for THAT image.

### Demo Video

https://github.com/user-attachments/assets/b44a32b3-6348-4b49-ae38-948d43df7d4b



### Rubric

Rubric file: [A6 Rubric.txt](./A6%20Rubric.txt)

```text
Grader: <TODO Your Name>, <TODO Your NetID>


Total:             +12
Deductions:   -TODO
—----------------
Final Score:        TODO


[Remember to fill out the A6 feedback form for the final +1 pt!]


——————


Comments:


<TODO: Add encouraging comments here! Point out some nice things about their implementation, and give constructive feedback in a few places if possible.>


——————


Deductions:


<TODO: Apply the correct deductions, then DELETE THIS TEXT>


General
* [-6] App does not compile nor launch, even if the grader attempted to fix any local Gradle issues.


Rendering Photos (2pts)
* [-2] Cat test photos (and other photos) do not show up.
* [-1] Cat test photo hardcoded; uploading photos (if implemented) does not render new photos.


Uploading Photos (2pts)
* [-2] Not implemented; clicking the upload photo card does not launch the photo picker.
* [-1] Not implemented with UIEvent (`pickMedia.launch` called directly)


Navigation (3pts)
* [-3] Cannot navigate at all to the Rating Screen.
* [-2] Clicking on an image does not navigate to the screen.
* [-1] Clicking on a particular image does not send the correct image ID through the navigation arguments.
* [-1] User does not automatically navigate 1 second after uploading a new image.


Rating Nav Args (3pts)
* [-1] No logic exists to load the image, such as photoRatingRepository.getImageFromId().
* [-1] No UIState field for image bitmap or other flow connecting the image bitmap to the UI.
* [-1] UI does not render the image given to it by the VM.
* [-1] See my Rating! button does not only become enabled when the image loads (should be greyed out until image loads)


Show the Ratings! (2pts)
* [-2] 5 ratings not displayed at all.
* [-1] Some ratings are missing.
* [-1] No animation exists at all for displaying the ratings. (lenient deduction)
```
