# Python Phishing URL Detection


**Python 3.11.9 _(Currently Using)_**




- Create a virtual environment
```bash
python -m venv zenv
source zenv/Scripts/activate # Windows
source zenv/bin/activate # Mac
```


- Install basic requirements
```bash
pip install -r requirements.txt

# OR INITIAL INSTALLATION 
pip install --upgrade pip
pip install --upgrade setuptools

pip install pandas whois httpx
pip install pycaret # It will take sometime.
```

### Replace Domains

```python
if __name__ == "__main__": 
    phishing_url_1 = 'https://bafybeifqd2yktzvwjw5g42l2ghvxsxn76khhsgqpkaqfdhnqf3kiuiegw4.ipfs.dweb.link/'
    phishing_url_2 = 'http://about-ads-microsoft-com.o365.frc.skyfencenet.com'
    real_url_1 = 'https://chat.openai.com'
    real_url_2 = 'https://github.com/'
    
    
    print(predict(phishing_url_1))
    print(predict(phishing_url_2))
    print(predict(real_url_1))
    print(predict(real_url_2))
```

### To Run

```bash
python main.py


# OUTPUT: {'prediction_label': 0, 'prediction_score': 68.39} 

# 0 = False | 1 True
```

---

### To Run GUI

```bash
pip install flask

python app.py
```




