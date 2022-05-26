<p align="center">
  <a href="#" target="_blank" rel="noopener noreferrer">
    <img src="/json.jpeg" width="300">
  </a>
</p>

# Welcome to Session 8

## Intall Git & Basic use

1. Install Git

    `windows` https://git-scm.com/download/win
    `macos`

        brew install git
    
    kiểm tra:
        
        git --version


2. Clone package 

        git clone <source>   
        cd <repo name>

3. Install package

        pip install -r requirements.txt
        

## Open web page
Home page
https://<user name>.github.io/



## Usage

**Basic command**
- `git init` Khởi tạo (thường khi tải về đã được khởi tạo rồi)
- `git clone` Tải 1 repo về
- `git add <file name>` Đưa file vào trạng thái lên sân khấu để theo dấu
- `git commit -m` save 1 version
- `git push origin main` main/master, đẩy lên remote repository
- `git pull` kéo các thay đổi về local

# Anaconda


**Tạo môi trường mới**
`conda create -n env_name [python=X.X] [LIST_OF_PACKAGES]`

`conda create --name py39_stock python=3.9 pandas requests`

**Kích hoạt**
`conda activate py39_stock`

=> `Sẽ hiện (py39_stock) ở terminal`

        **Note
        For  conda 4.6 and later versions on Linux/macOS/Windows, use
        conda activate my_env
        #For conda versions prior to 4.6 on Linux/macOS, use 
        source activate my_env
        #For conda versions prior to 4.6 on Windows, use 
        activate my_env

**Thoát môi trường**
`conda deactivate`

        Note:
        For  conda 4.6 and later versions on Linux/macOS/Windows, use
        conda deactivate
        #For conda versions prior to 4.6 on Linux/macOS, use 
        source deactivate
        #For conda versions prior to 4.6 on Windows, use 
        deactivate


**Liệt kê các môi trường đang có**
`conda env list`

**Liệt kê các package trong môi trường đang có**
`conda list`

**Cài đặt các package bổ sung**

`conda install pip`
`conda install numpy scipy pandas`

Conda tự động cài đặt các thư viện phụ thuộc (dependencies) giúp mình. Ví dụ thư viện scipy sử dụng numpy, “conda install scipy” sẽ tự động cài luôn numpy

**Update Packages**
`conda update package_name`

**Remove Packages**
`conda remove PACKAGE_NAME`

**Search a Package to Install**
`conda search *beautifulsoup*`

https://conda.io/projects/conda/en/latest/commands.html

**Share the List of Dependencies**
Đối với người dùng không sử dụng conda, cách tạo ra danh sách các package trong file requirements.txt:

`pip freeze > requirements.txt`

Sau đó có thể cài đặt tất cả package cần thiết:

`pip install -r requirements.txt`

## References

**Link** 

https://www.youtube.com/watch?v=NcoBAfJ6l2Q
https://www.w3schools.com/html/
https://www.freecodecamp.org/news/python-version-on-mac-update/

**Package phổ biến** 

requests - network
https://requests.readthedocs.io/en/latest/


fastapi - web framework  
https://fastapi.tiangolo.com/tutorial/first-steps/  
https://fastapi.tiangolo.com/tutorial/sql-databases/
https://towardsdatascience.com/fastapi-cloud-database-loading-with-python-1f531f1d438a

jinja template 
https://jinja.palletsprojects.com/en/3.0.x/templates/

plotly - chart  
https://plotly.com/javascript/  