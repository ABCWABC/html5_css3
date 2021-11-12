# html5_css3
학원 html, css _ layout1

<!DOCTYPE html>
<html>
    <head>
        <title>html5_css3</title>
        <style>
            * {
                box-sizing: border-box; 
                /* width 안에 padding, border 포함시켜서 사용 */
            }
            
            body {
                font-family: Arial;
                padding: 10px; /* top r b l */
                background: #f1f1f1;
            }
            
            .header {
                padding: 30px;
                text-align: center;
                background: #FFFFFF;
            }

            .header h1 {
                font-size: 50px;
            }

            .topnav {
                background-color: #333;
                overflow: hidden;          /*이걸해줘야지 배경색이 나타남*/
            }

            .topnav a {
                float: left;
                display: block;
                padding: 14px 16px;
                color: #f2f2f2;
                text-align: center;
                text-decoration: none;
            }

            .topnav a:hover {
                background-color: #ddd;
                color: black;
            }

            .leftcolumn {
                float: left;
                width: 75%;
                background-color: white;
                padding: 20px;
                margin-top: 20px;
            }

            .rightcolumn {
                float: left;
                width: 25%;
                background-color: white;
                padding: 20px;
                margin-top: 20px;
            }

            .fakeimg {
                background-color: #aaa;
                width: 100%;
                padding: 20px;
            }

            .card {
                border-color: pink;
                padding: 20px;
                margin-top: 20px;
            }

            .row::after {
                content: "";
                display: table;
                clear: both;
            }

            .footer {
                padding: 20px;
                text-align: center;
                background: #ddd;
                margin-top: 20px;
            }

            @media screen and (max-width: 800px) {
                .leftcolumn, .rightcolumn {   
                    width: 100%;
                    padding: 0;
                }
            }

            @media screen and (max-width: 400px) {
                .topnav a {
                    float: none;
                    width: 100%;
                }
            }

        </style>
    </head>
    <body>
        <div class="header">
            <h1>My Website</h1>
            <p>안녕하세요</p>
        </div>
        <div class="topnav">
            <a href="#">link1</a>
            <a href="#">link2</a>
            <a href="#">link3</a>
            <a href="#">link4</a>
        </div>

        <div class="row"> <!-- 메인을 감싸는 div 태그-->
            <div class="leftcolumn"><!-- 왼쪽을 감싸는 div 태그-->
                <div class="card">
                    <h2>TITLE HEADING</h2>
                    <h5>Title description, Dec 7, 2017</h5>
                    <div class="fakeimg" style="height: 200px;">  <!-- 이미지가 삽입된 div 태그-->
                        이미지
                    </div>
                    <P>Some text..</P>
                    <p>왼쪽상단 단락내용</p>
                </div>
                <div class="card">
                    <h2>TITLE HEADING</h2>
                    <h5>Title description, Sep 2, 2017</h5>
                    <div class="fakeimg" style="height: 200px;">  <!-- 이미지가 삽입된 div 태그-->
                        이미지
                    </div>
                    <P>Some text..</P>
                    <p>왼쪽하단 단락내용</p>
                </div>
            </div>
            <div class="rightcolumn"><!-- 오른쪽을 감싸는 div 태그-->
                <div class="card">
                    <h2>About me</h2>
                    <div class="fakeimg">
                        이미지
                    </div>
                    <div>
                        <p>Some text about me</p>
                    </div>
                </div>
                <div class="card">
                    <h3>Popular post</h3>
                    <div class="fakeimg" style="height: 100px;">이미지</div>
                    <div class="fakeimg" style="height: 100px;">이미지</div>
                    <div class="fakeimg" style="height: 100px;">이미지</div>
                </div>
                <div class="card">
                    <h3>Follow Me</h3>
                    <p>Some text..</p>
                </div>
            </div>
        </div>

        <div class="footer"> <!-- foot을 감싸는 div 태그-->
            <h2>footer</h2>
        </div>

    </body>
</html>
