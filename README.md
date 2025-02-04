# jubilant-funicular

This project fetches the latest 100 transactions for the Beacon Deposit Contract from Etherscan, saves the data in a JSON file, and displays it on a web page. The data is updated every hour using GitHub Actions, and the web page is published using GitHub Pages.

## Components

### Python Script

The Python script 

tx.py

 queries the Etherscan API to get the latest 100 transactions for the Beacon Deposit Contract and saves the data in `transactions.json`.

### GitHub Actions

A GitHub Actions workflow is set up to run the Python script every hour. The workflow is defined in main.yml


### HTML Page

The HTML page 

index.html

 displays the transaction data in a table format. The data is fetched from `transactions.json`.

### GitHub Pages

The HTML page is published using GitHub Pages at [https://draju1980.github.io/jubilant-funicular/](https://draju1980.github.io/jubilant-funicular/).

## Setup

1. **Clone the repository:**
    ```sh
    git clone https://github.com/draju1980/jubilant-funicular.git
    cd jubilant-funicular
    ```

2. **Install dependencies:**
    ```sh
    pip install -r requirements.txt
    ```

3. **Run the script:**
    ```sh
    python tx.py
    ```

4. **View the HTML page:**
    Open 

index.html

 in a web browser to view the transaction data.

## GitHub Actions Workflow

The GitHub Actions workflow is defined in 

main.yml

. It runs the Python script every hour and commits the updated `transactions.json` file to the repository.

## License

This project is licensed under the MIT License. See the LICENSE file for details.