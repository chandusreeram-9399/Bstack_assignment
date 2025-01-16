# python-selenium-browserstack
Run python tests on browserstack using the SDK.

## Prerequisite
```
python3 should be installed
```

## Setup
* Clone the repo
```
git clone https://github.com/chandusreeram-9399/.git
```

* Install packages through requirements.txt
```
pip3 install -r requirements.txt
```

* Virtual environment(Recommended)
```
python -m venv env
env\Scripts\activate
```

## API
* url = "https://rapid-translate-multi-traduction.p.rapidapi.com/t"

* headers = {
```
    "x-rapidapi-key": "API_KEY",
    "x-rapidapi-host": "rapid-translate-multi-traduction.p.rapidapi.com",
    "Content-Type": "application/json"
```
}

## Set BrowserStack Credentials
* Add your BrowserStack username and access key in the `browserstack.yml` config file.
* You can also export them as environment variables, `BROWSERSTACK_USERNAME` and `BROWSERSTACK_ACCESS_KEY`:

#### For Windows
```
BROWSERSTACK_USERNAME=<browserstack-username>
BROWSERSTACK_ACCESS_KEY=<browserstack-access-key>
```

## Running tests
* Run sample test:
  - To run the sample test across platforms defined in the `browserstack.yml` file, run:
    ```
    browserstack-sdk ./tests/test.py
    ```
  
  - To run the script on your local machine or any editor:
    ```
    ./tests/localmachine.py
    ```
