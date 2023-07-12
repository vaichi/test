You need to install the nltk and transformers modules using pip and download the English vocabulary data using nltk.download('words'). The BERT model will be downloaded automatically when you run the code for the first time.


1. `nltk` module: It is used for natural language processing tasks, such as accessing word resources like the English vocabulary.

2. `nltk.corpus.words` module: It provides access to a list of English words that can be used for spell checking and word suggestion.

3. `transformers` module: It is a library provided by Hugging Face for working with pre-trained models in natural language processing, including BERT.

4. `BertTokenizer.from_pretrained('bert-base-uncased')`: It initializes a BERT tokenizer from the pre-trained 'bert-base-uncased' model. The tokenizer is used for tokenizing the input text.

5. `perform_token_healing(text)`: This function performs the main task of error correction and token healing. It tokenizes the input text using the BERT tokenizer, applies custom error rules, checks for misspelled words, suggests corrections based on the context, and prompts the user for feedback. Finally, it returns the corrected text.

6. `is_word(token)`: This function checks if a token (word) exists in the English vocabulary. It uses the `words.words()` from the `nltk.corpus` module.

7. `suggest_word(token, tokens)`: This function suggests alternative words for a given token based on the context. It searches for the token in the list of BERT tokens and collects the surrounding tokens as suggestions.

8. `apply_custom_error_rules(token)`: This function applies custom error rules to specific tokens. It checks for predefined custom rules and returns the corrected word if a match is found, or None if no rule applies.

9. `while True` loop: It creates an interactive loop where the user can enter sentences for error correction. The loop continues until the user enters 'exit'.

10. Sample inputs and outputs: These are examples provided to showcase how the code corrects misspelled words, applies custom error rules, and suggests word alternatives based on the context.



sample inputs and outputs:

Input: "I am writting a lettter to my frend."
Output: "I am writing a letter to my friend."

Input: "The techer was very knowlegeable and helpfull."
Output: "The teacher was very knowledgeable and helpful."

Input: "I wana go to the park tommorow."
Output: "I want to go to the park tomorrow."

Input: "He is a good persn."
Output: "He is a good person."

Input: "I saw a beutiful sunrize this morning."
Output: "I saw a beautiful sunrise this morning."

Input: "I can't beleave I did that."
Output: "I can't believe I did that."

Input: "Im gonna be late for the meating."
Output: "I'm going to be late for the meeting."






Congrats! 🎉

If you made it here then you have passed our initial screening. Welcome to second round of your interview.

During this round, we will evaluate your ability to handle new and intricate learning challenges. Choose one of the following assignments. But don't spend no more than 12 hours working on it. After 12 hours, please submit your progress, regardless of the extent of completion. Feel free to generate code using AI tools and chat apps like chatgpt, bing chat, code copilots, codium etc.

To access the assignment details, kindly visit the ***#second-round*** channel . If you have any questions ask in the ***#interview-doubts*** channel.

Discord link -<https://discord.gg/uTYkFDS8>

To create a pull request for a public git repo, you need to follow these steps:

-   Fork the repo that you want to contribute to. This will create a copy of the repo under your own GitHub account. You can fork a repo by clicking the **Fork** button on the top right corner of the repo page.
-   Clone your forked repo to your local machine. You can do this by running **`git clone <https://github.com/your-username/repo-name.git`**> in your terminal, where **`your-username`** is your GitHub username and **`repo-name`** is the name of the repo you forked.
-   Create a new branch for your changes. You can do this by running **`git checkout -b branch-name`**, where **`branch-name`** is a descriptive name for your branch.
-   Make your changes in the new branch. You can use any code editor or IDE that you prefer. You can also use GitHub Desktop to manage your changes.
-   Add and commit your changes to the new branch. You can do this by running **`git add .`** to stage all your changes and **`git commit -m "message"`** to commit them with a message, where **`message`** is a brief summary of what you did.
-   Push your changes to your forked repo on GitHub. You can do this by running **`git push origin branch-name`**, where **`branch-name`** is the name of your branch.
-   Create a pull request from your forked repo to the original repo. You can do this by going to your forked repo on GitHub and clicking the **Compare & pull request** button. This will open a page where you can review your changes and add a title and a description for your pull request. You can also link your pull request to an issue if there is one related to your changes. Then click **Create pull request** to submit it.

That's it! You have created a pull request for a public git repo. Now you need to wait for the maintainers of the original repo to review and merge your pull request. They might also ask you for some feedback or changes before merging it. You can communicate with them through the comments section of your pull request.
