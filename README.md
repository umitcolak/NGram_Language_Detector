# NGram_Language_Detector

**NGram Language Detector** is a Python project that generates language profiles based on n-gram analysis and uses these profiles to classify text into different languages. The project includes functionalities for creating n-grams, counting their frequencies, storing language profiles, and evaluating text classification.

## How It Works

### 1. N-Gram Models:
- **N-Gram Creation**: The program creates n-grams from text, where n can vary (e.g., 1-gram, 2-gram, up to 5-gram). N-grams are sequences of n characters extracted from the text with padding.
- **Text Cleaning**: The text is cleaned by removing non-alphabetic characters, converting to lowercase, and removing extra spaces.

### 2. Text Analysis:
- **N-Gram Frequency Counting**: Counts the frequency of each n-gram in the text.
- **Language Profile Creation**: Reads text files, generates n-grams, counts their frequencies, and stores the top n-grams as language profiles.
- **Language Classification**: Compares n-gram profiles of a new text against stored language profiles to determine the closest match.

## Techniques Applied

### a. Tokenization:
The text is broken down into manageable pieces called tokens (usually characters or words). This involves removing punctuation and converting all text to lower case to ensure uniformity.

### b. Probability Calculation:
- For n-grams, the probability of each sequence is calculated based on their frequency of occurrence in the training data.

### c. Model Storage:
The n-gram frequencies are stored in a data structure (such as a dictionary) where each key is an n-gram, and the value is its frequency.

## Training the Model

1. **Data Collection**: Compile a large corpus of text data that is representative of the language or style you wish to generate.
2. **Preprocessing**: Apply tokenization and text cleaning to prepare the data.
3. **Frequency Counting**: Count how often each n-gram occurs in the corpus.
4. **Profile Storage**: Store the n-gram frequencies in files for each language.

## Using the Program

### 1. Load and Create N-Gram Profiles
- Load or create n-gram profiles from text files for different languages.
- Save the profiles to individual text files.

### 2. Generate and Analyze N-Gram Profiles
- Generate n-gram profiles for new texts.
- Compare these profiles with stored language profiles to classify the text.

## Practical Applications

This tool can be extremely useful in various domains:
- **Language Classification**: Identifying the language of a given text.
- **Text Analysis**: Analyzing text patterns and structures using n-grams.
- **Content Creation**: Assisting in understanding language usage and frequency patterns.
