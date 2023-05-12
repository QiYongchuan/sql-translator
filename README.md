## 中文版本地安装说明

原版README说明在下面，其实已经很详细了，跟着步骤无脑一步一步进行就可以了。为了照顾仍然不成功的同学，特地推出啰嗦版安装流程。

## 🛠️ 本地安装（也就是安装到你的电脑上，只需要看下面的就可以了，按道理需要部署到Dooker上的不会看这个的）

### 本地开发环境

0. 先在你电脑的C或D盘新建一个文件夹，取一个你喜欢的名字。
比如这样：
 ![image](https://github.com/QiYongchuan/sql-translator/assets/105039020/ba97f969-340c-42db-be0a-7c8225cc4831)
 
1. 下载这段程序的代码：
   1.1 最简单的方法是使用git下载，右键你的文件夹，然后点击在终端中打开，就进入终端了，进而输入命令：
   ```bash
    git clone https://github.com/whoiskatrin/sql-translator.git
    ```
    但我猜有的人电脑上没有下载git？
    
 2.下载完成后接着在命令行输入命令：意思是进入文件夹，安装包
    ```bash
    cd sql-translator
    npm install
    ```
3.  接着输命令

    ```bash
    npm run build
    ```

4.把你的OPENAI 的API key 放到 .env 文件中, 如果没有api的key就点这里获取一个 [here](https://beta.openai.com/account/api-keys):
     
     建议可以将这个文件夹在vscode中打开，方便填写。
     ![image](https://github.com/QiYongchuan/sql-translator/assets/105039020/43ab7944-d054-42c4-8fb7-db41fd096847)

     ![image](https://github.com/QiYongchuan/sql-translator/assets/105039020/7534cd3f-582b-40ca-8525-c883a8fb697e)
     
5. 启动本地服务器:在命令行里输入下面的命令
    ```bash
    npm start
    ```
    
6. 然后就启动了
![image](https://github.com/QiYongchuan/sql-translator/assets/105039020/33ceb18e-e127-4cf7-978a-03b4e76f3bae)
![image](https://github.com/QiYongchuan/sql-translator/assets/105039020/9e0ba046-8690-41bb-9388-0d04ff69a09c)

————————————————————————————————————————————————————————————————————————————————————————————————————————————————————————————————————————————————————————————

这里是原来英文版的说明：

<h1 align="center">SQL Translator<br>(SQL to Natural Language and Natural Language to SQL)</h1>

Welcome to the SQL and Natural Language Translator! This tool is designed to make it easy for anyone to translate SQL (Structured Query Language) commands into natural language and vice versa. SQL is a programming language used to manage and manipulate data in relational databases, and while it's a powerful tool, it can also be quite complex and difficult to understand. On the other hand, natural language is the language that we speak and write in everyday life, and it's often the preferred way to communicate for people who are not familiar with technical jargon.

With the SQL and Natural Language Translator, you don't need to be a SQL expert to understand what's going on in your database, or to write SQL queries. You can simply type in your query in natural language and get the corresponding SQL code, or type in your SQL code and get a human-readable translation.This project is 100% free and open source.


## 🌟 Features

- Dark mode
- Lowercase/uppercase toggle
- Copy to clipboard
- SQL syntax highlighting
- Schema awareness (beta)
- Query history


## 📖 How to use:

Using the SQL to Natural Language Translator is easy. Simply navigate to the tool's website and choose whether you want to translate from natural language to SQL or from SQL to natural language. Then, type in your query and hit the "translate" button. The tool will generate the corresponding code or text and display it on the screen. 
You can press the 'reverse' button to give input as Natural Language and get SQL queries in response


## 🎯 Roadmap

- [ ] Functions
- [ ] Procedures


## 🛠️ Installation

### Local Development Environment

1. Clone the repository:

    ```bash
    git clone https://github.com/whoiskatrin/sql-translator.git
    ```

2. Install the required packages:

    ```bash
    cd sql-translator
    npm install
    ```

3. Build the application:

    ```bash
    npm run build
    ```

4. Input your OPENAI API key in the .env file, you can get your API key [here](https://beta.openai.com/account/api-keys):

    ```bash
    OPENAI_API_KEY=$YOUR_API_KEY
    ```

5. Start the development server:

    ```bash
    npm start
    ```

### Docker Compose

1. Clone the repository:

    ```bash
    git clone https://github.com/whoiskatrin/sql-translator.git
    ```

2. Input your OPENAI API key in the .env.production file, you can get your API key [here](https://beta.openai.com/account/api-keys):

    ```bash
    OPENAI_API_KEY=$YOUR_API_KEY
    ```

3. Start the development server:

    ```bash
    docker-compose up
    ```

## 🖥️ Usage

Once the development server is running, you can access the application by navigating to `http://localhost:3000` in your web browser.

Enter a natural language query in the input box and click "Translate" to generate the corresponding SQL code. The generated SQL code will be displayed in the output box.

## 👥 Contributing

Contributions to SQL Translator are welcome and encouraged! To contribute, please follow these steps:

1. Fork the repository
2. Create a new branch
3. Make your changes
4. Push your changes to your fork
5. Submit a pull request

## 📜 License

SQL Translator is released under the MIT [License](LICENSE).
