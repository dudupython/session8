<p align="center">
  <a href="#" target="_blank" rel="noopener noreferrer">
    <img src="/json.jpeg" width="300">
  </a>
</p>

# Welcome to repository

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
- `git init` Khởi tạo
- `git clone` Tải 1 repo về
- `git add <file name>` Đưa file vào trạng thái lên sân khấu để theo dấu
- `git commit -m` save 1 version
- `git push origin main` main/master, đẩy lên remote repository


## Explaination 

**Notes**:

- Pydantic model (data validation) khác với sqlAlchemy model (class & intanstant interact with database)
- Pydantic model trong schemas.py, SQLAlchemy model trong models.py của từng Feature/Project
- Mỗi tính năng sẽ có model/database.py riêng, DB chung ở database/core.py    
- `#database/core.py`  Create SQLAlchemy models from the `Base` class and import to  models.py of each Project  
- `orm_mode = True` - Pydantic's orm_mode will tell the Pydantic model to read the data even if it is not a dict  
- `SessionLocal` - instant class of database session  
- `Session` from  `sqlalchemy.orm` - The session is an SQLAlchemy object used to communicate with SQLite in the Python example programs
- `Alembic` module - initialize your database (create tables, etc) & migrations

- Flow: Add job schedule, đến thời điểm triggle (`cron`, `interval`) sẽ vào hàng đợi của Celery
- Mỗi lần thay đổi logic ở `@task` của celery phải reset lại worker
- Không cần phải restart server khi hẹn giờ cho task

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