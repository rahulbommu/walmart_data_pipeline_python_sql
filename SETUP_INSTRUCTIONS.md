# 🛠️ Setup Instructions & Terminal Commands

## 📋 Prerequisites
- Python 3.8 or higher
- Basic understanding of command line/terminal
- Text editor or IDE (VS Code recommended)

---

## 🖥️ Environment Setup

### macOS Terminal Commands
```bash
# Install Homebrew if not installed
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

# Install Python (if not installed)
brew install python

# Verify Python installation
python3 --version
```

### Windows Command Prompt Commands
```cmd
:: Download and install Python from python.org
:: Make sure to check "Add Python to PATH" during installation

:: Verify Python installation
python --version

:: Install pip if not installed (usually comes with Python)
python -m ensurepip --upgrade
```

### Linux (Ubuntu/Debian) Commands
```bash
# Update package list
sudo apt update

# Install Python and pip
sudo apt install python3 python3-pip

# Verify installation
python3 --version
pip3 --version
```

---

## 📦 Project Setup

### 1. Clone the Repository
```bash
git clone <repository-url>
cd walmart_data_pipeline_python_sql
```

### 2. Install Required Libraries
```bash
# Install all dependencies
pip install -r requirements.txt

# Or install individually:
pip install pandas pymysql sqlalchemy psycopg2-binary jupyter numpy
```

### 3. Verify Installation
```bash
# Test Python imports
python3 -c "import pandas, pymysql, sqlalchemy, psycopg2; print('All libraries installed successfully!')"
```

---

## 🔗 Kaggle API Setup (Optional)

If you want to download datasets directly from Kaggle:

### 1. Create Kaggle Account
- Go to [kaggle.com](https://www.kaggle.com) and create an account
- Go to Account settings → API → Create New API Token
- This downloads `kaggle.json` file

### 2. Configure Kaggle API

#### macOS/Linux:
```bash
# Create Kaggle directory
mkdir ~/.kaggle

# Move kaggle.json to the directory
mv ~/Downloads/kaggle.json ~/.kaggle/

# Set proper permissions
chmod 600 ~/.kaggle/kaggle.json

# Install Kaggle package
pip install kaggle
```

#### Windows:
```cmd
:: Create Kaggle directory
mkdir %USERPROFILE%\.kaggle

:: Move kaggle.json (adjust path if needed)
copy %USERPROFILE%\Downloads\kaggle.json %USERPROFILE%\.kaggle\

:: Install Kaggle package
pip install kaggle
```

### 3. Test Kaggle API
```bash
# List available datasets (should work if configured correctly)
kaggle datasets list

# Download the Walmart dataset (example)
kaggle datasets download -d najir0123/walmart-10k-sales-datasets
```

---

## 🗄️ Database Setup (Optional)

### MySQL Setup

#### macOS (using Homebrew):
```bash
# Install MySQL
brew install mysql

# Start MySQL service
brew services start mysql

# Secure installation
mysql_secure_installation
```

#### Windows:
1. Download MySQL installer from [mysql.com](https://dev.mysql.com/downloads/installer/)
2. Run installer and follow setup wizard
3. Remember the root password you set

#### Linux (Ubuntu/Debian):
```bash
# Install MySQL
sudo apt install mysql-server

# Secure installation
sudo mysql_secure_installation

# Start MySQL service
sudo systemctl start mysql
```

### PostgreSQL Setup

#### macOS (using Homebrew):
```bash
# Install PostgreSQL
brew install postgresql

# Start PostgreSQL service
brew services start postgresql

# Create database user
createuser -s postgres
```

#### Windows:
1. Download PostgreSQL installer from [postgresql.org](https://www.postgresql.org/download/windows/)
2. Run installer and follow setup wizard
3. Remember the password you set

#### Linux (Ubuntu/Debian):
```bash
# Install PostgreSQL
sudo apt install postgresql postgresql-contrib

# Start PostgreSQL service
sudo systemctl start postgresql

# Switch to postgres user
sudo -u postgres psql
```

---

## 🚀 Running the Project

### 1. Start Jupyter Notebook
```bash
# Navigate to project directory
cd walmart_data_pipeline_python_sql

# Start Jupyter Notebook
jupyter notebook

# Your browser should open with the notebook interface
# Click on 'project.ipynb' to open the main notebook
```

### 2. Alternative: Use Jupyter Lab
```bash
# Install Jupyter Lab (more modern interface)
pip install jupyterlab

# Start Jupyter Lab
jupyter lab
```

### 3. Run Python Scripts Directly
```bash
# If you prefer running Python files directly
python3 -c "
import pandas as pd
df = pd.read_csv('Walmart.csv')
print(f'Dataset loaded: {df.shape[0]} rows, {df.shape[1]} columns')
print('Setup successful!')
"
```

---

## ✅ Verification Checklist

Before starting the analysis, make sure:

- [ ] Python 3.8+ is installed and accessible
- [ ] All required libraries are installed (`pip list` shows pandas, pymysql, etc.)
- [ ] Jupyter Notebook starts without errors
- [ ] You can load the Walmart.csv file
- [ ] (Optional) Database connections work if you plan to use them
- [ ] (Optional) Kaggle API is configured if you want to download data

### Quick Test Script
```python
# Save this as test_setup.py and run: python3 test_setup.py
try:
    import pandas as pd
    import pymysql
    import sqlalchemy
    import psycopg2
    print("✅ All required libraries imported successfully!")
    
    # Test data loading
    df = pd.read_csv('Walmart.csv', encoding_errors='ignore')
    print(f"✅ Data loaded: {df.shape[0]} rows, {df.shape[1]} columns")
    
    print("🎉 Setup is complete! You're ready to start analyzing.")
    
except ImportError as e:
    print(f"❌ Missing library: {e}")
    print("Run: pip install -r requirements.txt")
    
except FileNotFoundError:
    print("❌ Walmart.csv not found in current directory")
    print("Make sure you're in the project directory")
    
except Exception as e:
    print(f"❌ Error: {e}")
```

---

## 🆘 Common Issues & Solutions

### Issue: "pandas not found" or similar import errors
**Solution**: 
```bash
pip install --upgrade pip
pip install -r requirements.txt
```

### Issue: "Permission denied" on macOS/Linux
**Solution**: 
```bash
pip install --user -r requirements.txt
```

### Issue: Jupyter Notebook won't start
**Solution**: 
```bash
pip install --upgrade jupyter
jupyter notebook --generate-config
```

### Issue: Database connection errors
**Solution**: 
- Make sure database server is running
- Check connection parameters (host, port, username, password)
- For learning purposes, you can skip database parts and focus on CSV analysis

### Issue: Kaggle API not working
**Solution**: 
- Verify kaggle.json is in the correct location
- Check file permissions: `chmod 600 ~/.kaggle/kaggle.json`
- Test with: `kaggle datasets list`

---

## 🎯 Next Steps

Once setup is complete:

1. **Start with the guides**: Read `PROJECT_SUMMARY.md` for an overview
2. **Open the notebook**: Run `jupyter notebook` and open `project.ipynb`
3. **Run cell by cell**: Execute each code cell and observe the outputs
4. **Explore the data**: Try modifying queries and see what happens
5. **Read SQL files**: Examine the business analysis queries

**Happy analyzing!** 🚀