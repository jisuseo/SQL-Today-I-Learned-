# **Today I learned**
## 2024
<details>
  <summary>
    <h2>SEP.2024</h2>
    </summary>
<details>
  <summary>
   <h4>08.SEP </h4>
  </summary>
  - Learned basic git commands <br>
  - Practiced Git commit and push <br>
      <details>
        <summary> 
        - SQL
        </summary>
          - Relational Database <br>
        - is declarative <br>
        <details>
        <summary>
          1.sqlite
        </summary>
          - scoop <br>
          - powershell <br>
          - Scoop is installed by default without admin privileges <br>
          - through Download manager 'Scoop'
          <pre><code>scoop bucket add main <br>
scoop install main/sqlite </code></pre>
  - for use sqlite write <pre><code>sqlite3<br></code></pre>
        </details>
    </details>
</details>
  
<details>
  <summary>
    <h4>09.SEP</h4>
  </summary>
  - Continuing SQLite study through Scoop following yesterday <br>
  - Enter at the specified path in PowerShell
  <pre><code>New-Item database.db</code></pre>
  - Theory about Data Definition Language (DDL)
  - comments <pre><code> -- </code></pre>
  - table = Sheet(Excel)
  - sqlite3
  <pre><code>create table movies (
(x1...> titel,
(x1...> released,
(x1...> overview,
(x1...> rating,
(x1...> director
(x1...> );</code></pre>
  - to list all the tables in the database 
  <pre><code>.tables</code></pre>
  - to check the structure of the 'movies' table 
  <pre><code>PRAGMA table_info(movies);</code></pre>
  - INSERT INTO ... VALUES
  <pre><code>INSERT INTO movies VALUES (
(x1...> 'The Godfather',
(x1...> 1980,
(x1...> 'The best movie in the world',
(x1...> 10,
(x1...> 'F.F.C'
(x1...> );</code></pre>
  - to show
  <pre><code>SELECT * FROM movies;</code></pre>
  - to remove
  <pre><code>DROP TABLE movies;</code></pre>
  - To leave a value empty, input NULL or use
  <pre><code>INSERT INTO movies (title, rating) VALUES ('TLOTR 2', 10);
</code></pre>
  - to value type INTEGER (1,2,3...), REAL (1.2, 9.7 ...), BLOB (image) (binary large object)
  
</details>
<details>
  <summary>
    <h4>11.SEP</h4>
  </summary>
- constraint (제약조건) - A constraint helps control the data that can be entered into a column <br>
- ex)
<pre><code>CREATE TABLE movies (<br>
title TEXT UNIQUE NOT NULL, <br>
released INTEGER NOT NULL, <br>
overview text NOT NULL, <br>
rating REAL NOT NULL, <br>
director TEXT, <br>
for_kids INTEGER NOT NULL DEFAULT 0 <br>
) STRICT;</code></pre>
</code></pre>
  
</details>
<details>
  <summary>
    <h4>12.SEP</h4>
  </summary>
- sqlite3 start
<<<<<<< HEAD
<pre><code>sqlite3 database.db</code></pre> <br>
- commit with visual studio code

=======
  <pre><code>sqlite3 database.db</code></pre>
- configure user name and email in git <br>
  <pre><code>git config --global user.name "Your Name"
git config --global user.email "your-email@example.com</code></pre>
- to check the configuration
  <pre><code>git config --global --list</code></pre>
>>>>>>> 28fbadc5581444668e912df8330ded61eb23462a
- CHECK Constraint (강력한 제약조건)
- 
  
</details>
<details>
  <summary>
    <h4>15.SEP</h4>
  </summary>
  <pre><code>
  - git add . <br>
- git commit -m "message" <br>
- git push
# At once
-git add . && git commit -m "메시지" && git push origin main
  </code></pre>
  - pip install poetry <br>
  - poetry new "project name" <Br>
  - poetry init <br>
  - poetry python verseion <br>
  ==> <pre><code>python = ">=3.12,<4.0"</code></pre>
    <pre><code>
    - pip install pandas <br>
    - pip install plotly <Br>
    - pip install numpy <br>
    - import pandas as pd <br>
    - df1 = pd.read_csv("path with Filename") <br>
    df1.head()<br>
    df1.FraudFound_p.unique() # to find unique Value <Br>
    df1.PolicyType.unique() # <br>
    df1.shape <br>
    df1.nunique() <br>
    df1.info() <br> 
    df1.describe() <br>
    df1.isnull().sum() # 0 means not null in all Values <br>
    </code></pre>
    - functionization
    <pre><code>def count_plot(df1, column):
    fig = px.histogram(df1, x=column, title=f"Count plot of {column}",
                 category_orders={column:df1[column].value_counts().index})
    fig.show()
    return fig <br>
    f=countp_plot(df1, "Make")
    </code></pre>
</details>
</details>
