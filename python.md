# Python

Create virtual environment, install requirements

```bash
clone git@github.com:USERNAME/REPOSITORY_NAME.git
cd REPOSITORY_NAME
# python version should be 3.???.* something
python3 --version
python3 -m venv venv
source venv/bin/activate
# we need new version of pip for requirements.txt
pip install --upgrade pip
pip install -r requirements.txt
```

---

find out type of the variable

```python
type(VARIABLE)
```

---

print current working directory (from which the script is being run)

```python
import os
print(os.getcwd())
```

---