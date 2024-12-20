# YDP-S1-S2

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Big Five Personality Test</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
            background-color: #f9f9f9;
            color: #1b7135;
        }
        h1 {
            color: #2c3e50;
        }
        p {
            margin: 15px 0;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 20px;
            background-color: #fff;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        th, td {
            border: 1px solid #ddd;
            padding: 8px;
            text-align: left;
        }
        th {
            background-color: #1b5c36;
            color: #fff;
            font-weight: bold;
        }
        tr:nth-child(even) {
            background-color: #f2f2f2;
        }
        tr:hover {
            background-color: #eaf1f8;
        }
        td input[type="number"] {
            width: 100%;
            padding: 8px;
            font-size: 16px;
            border: 1px solid #ccc;
            border-radius: 4px;
        }
        td input[type="number"]:focus {
            border-color: #3498db;
            outline: none;
            box-shadow: 0 0 4px rgba(219, 158, 52, 0.8);
        }
        @media screen and (max-width: 300px) {
            table {
                display: block;
                overflow-x: scroll;
                white-space: nowrap;
            }
            th, td {
                font-size: 14px;
                padding: 6px;
            }
            td input[type="number"] {
                font-size: 14px;
                padding: 6px;
            }
        }
        .result-button {
            display: inline-block;
            margin-top: 20px;
            padding: 12px 20px;
            font-size: 16px;
            color: #fff;
            background-color: #d08c0f;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            text-transform: uppercase;
            font-weight: bold;
            transition: background-color 0.3s ease, transform 0.2s ease;
        }
        .result-button:hover {
            background-color: #2980b9;
            transform: translateY(-2px);
        }
        .result-button:active {
            background-color: #c89122;
            transform: translateY(1px);
        }
    </style>
</head>
<body>
    <h1>Big Five Personality Test</h1>
     <p>Доорх хүснэгтэд 1-50 хүртэлх асуулт тус бүрийг 1-5 хүртэлх оноогоор үнэлнэ. <br>
        1= санал нийлэхгүй <br> 2= бага зэрэг санал нийлэхгүй<br> 3= төвийг сахисан<br> 4= бага зэрэг санал нийлж байна <br> 5= санал нийлж байна гэсэн оноонуудаас сонгон баруун талын хоосон нүдэнд тэмдэглэнэ үү. 
        </p>
    <form id="testForm">
        <table>
            <thead>
                <tr>
                    <th>Асуулт</th>
                    <th>Оноо (1-5)</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>1. Би бол үдэшлэгийн гол хүн.</td>
                    <td><input type="number" name="q1" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>2. Би бусдын төлөө санаа зовох нь бага.</td>
                    <td><input type="number" name="q2" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>3. Би үргэлж бэлтгэлтэй байдаг.</td>
                    <td><input type="number" name="q3" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>4. Би стресст амархан өртдөг.</td>
                    <td><input type="number" name="q4" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>5. Би үгийн баялаг сайтай.</td>
                    <td><input type="number" name="q5" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>6. Би тийм ч их ярьдаггүй.</td>
                    <td><input type="number" name="q6" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>7. Би хүмүүсийн талаар сонирхдог.</td>
                    <td><input type="number" name="q7" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>8. Би өөрийнхөө эд зүйлсэд харам.</td>
                    <td><input type="number" name="q8" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>9. Би ихэнхдээ амар тайван байдаг.</td>
                    <td><input type="number" name="q9" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>10. Би хийсвэр ухагдахууныг ойлгохдоо тааруу.</td>
                    <td><input type="number" name="q10" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>11. Би хүмүүсийн дунд чөлөөтэй байж чаддаг.</td>
                    <td><input type="number" name="q11" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>12. Би хүмүүсийг доромжилдог.</td>
                    <td><input type="number" name="q12" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>13. Би нарийн зүйлсэд анхаарал хандуулдаг.</td>
                    <td><input type="number" name="q13" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>14. Би аливаа зүйлсэд санаа зовдог.</td>
                    <td><input type="number" name="q14" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>15. Би уран сэтгэмж сайтай.</td>
                    <td><input type="number" name="q15" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>16. Би анхаарлын төвд байдаггүй.</td>
                    <td><input type="number" name="q16" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>17. Би бусдын мэдрэмжийг мэдэрч чаддаг.</td>
                    <td><input type="number" name="q17" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>18. Би аливаа зүйлийг замбараагүй болгодог.</td>
                    <td><input type="number" name="q18" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>19. Би сэтгэлээр унах нь ховорхон.</td>
                    <td><input type="number" name="q19" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>20. Би хийсвэр санааг сонирхдоггүй.</td>
                    <td><input type="number" name="q20" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>21. Би харилцан яриаг эхлүүлдэг.</td>
                    <td><input type="number" name="q21" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>22. Би бусдын асуудлыг сонирхдоггүй.</td>
                    <td><input type="number" name="q22" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>23. Би аливаа ажлыг цаг алдалгүй дуусгаж чаддаг.</td>
                    <td><input type="number" name="q23" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>24. Би амархан сатаардаг.</td>
                    <td><input type="number" name="q24" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>25. Би гайхалтай шинэ зүйлсийг санаачилдаг.</td>
                    <td><input type="number" name="q25" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>26. Би хэлэх зүйл багатай байдаг.</td>
                    <td><input type="number" name="q26" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>27. Би зөөлөн сэтгэлтэй.</td>
                    <td><input type="number" name="q27" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>28. Би аливаа зүйлийг зохих байранд нь буцааж тавихаа мартдаг.</td>
                    <td><input type="number" name="q28" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>29. Би амархан бухимддаг.</td>
                    <td><input type="number" name="q29" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>30. Би тийм ч сайн уран төсөөлөлтэй биш.</td>
                    <td><input type="number" name="q30" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>31. Би үдэшлэгт маш олон хүмүүстэй ярилцдаг.</td>
                    <td><input type="number" name="q31" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>32. Би бусдын талаар үнэхээр сонирхдоггүй.</td>
                    <td><input type="number" name="q32" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>33. Би хэв журамд дуртай.</td>
                    <td><input type="number" name="q33" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>34. Би ааш зангаа өөрчлөх нь олон.</td>
                    <td><input type="number" name="q34" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>35. Би аливааг хурдан ойлгодог.</td>
                    <td><input type="number" name="q35" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>36. Би өөртөө бусдын анхаарлыг татах дүргүй.</td>
                    <td><input type="number" name="q36" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>37. Би бусдад цаг гаргадаг.</td>
                    <td><input type="number" name="q37" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>38. Би үүрэг хариуцлагаас зайлсхийдэг.</td>
                    <td><input type="number" name="q38" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>39. Би байнга сэтгэл санааны тогтворгүй байдалд байдаг. </td>
                    <td><input type="number" name="q39" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>40. Би хүнд үгнүүд ашигладаг.</td>
                    <td><input type="number" name="q40" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>41. Би олны анхаарлын төвд байхаас санаа зовдоггүй.</td>
                    <td><input type="number" name="q41" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>42. Би бусдын сэтгэл хөдлөлийг мэдэрдэг.</td>
                    <td><input type="number" name="q42" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>43. Би аливаа хуваарийг дагаж мөрддөг.</td>
                    <td><input type="number" name="q43" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>44. Би амархан уурладаг.</td>
                    <td><input type="number" name="q44" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>45. Би аливаа зүйлийг тунгаан бодоход цаг зарцуулдаг.</td>
                    <td><input type="number" name="q45" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>46. Би танихгүй хүмүүсийн дэргэд чимээгүй байдаг.</td>
                    <td><input type="number" name="q46" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>47. Би хүмүүсийг тайвшруулдаг.</td>
                    <td><input type="number" name="q47" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>48. Би ажилдаа шаардлага тавьдаг.</td>
                    <td><input type="number" name="q48" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>49. Би ихэнх тохиолдолд сэтгэлээр унадаг.</td>
                    <td><input type="number" name="q49" min="1" max="5" required></td>
                </tr>
                <tr>
                    <td>50. Би шинэ санаагаар дүүрэн.</td>
                    <td><input type="number" name="q50" min="1" max="5" required></td>
                </tr>

            </tbody>
        </table>
        <button type="submit" class="result-button">Үр дүн</button>
    </form>

    <script>
  document.addEventListener('DOMContentLoaded', () => {
    const inputs = Array.from(document.querySelectorAll('input[type="number"]'));
    inputs.forEach((input, index) => {
        input.addEventListener('input', () => {
            if (index < inputs.length - 1 && input.value !== '') {
                inputs[index + 1].focus();
            }
        });
    });
});

        document.getElementById("testForm").addEventListener("submit", function (event) {
            event.preventDefault();
            const formData = new FormData(event.target);

            const scores = {};
            formData.forEach((value, key) => {
                scores[key] = parseInt(value);
            });
            const O = 8 + scores.q5 - scores.q10 + scores.q15 - scores.q20 + scores.q25 - scores.q30 + scores.q35 + scores.q40 + scores.q45 + scores.q50;
            const C = 14 + scores.q3 - scores.q8 + scores.q13 - scores.q18 + scores.q23 - scores.q28 + scores.q33 - scores.q38 + scores.q43 + scores.q48;
            const E = 20 + scores.q1 - scores.q6 + scores.q11 - scores.q16 + scores.q21 - scores.q26 + scores.q31 - scores.q36 + scores.q41 - scores.q46;
            const A = 14 - scores.q2 + scores.q7 - scores.q12 + scores.q17 - scores.q22 + scores.q27 - scores.q32 + scores.q37 + scores.q42 + scores.q47;
            const N = 38 - scores.q4 + scores.q9 - scores.q14 + scores.q19 - scores.q24 - scores.q29 - scores.q34 - scores.q39 - scores.q44 - scores.q49;
        

            const descriptions = {
                O: `• Openness to Experience (O) – <b>Нээлттэй хэв шинж</b> 
                Шинэ туршлага, оюуны эрэл хайгуул хийдэг төрлийн зан чанар юм.`,
                C: `• Conscientiousness (C) – <b>Хариуцлагатай зарчимч хэв шинж</b>
                Шударга, ажилсаг хүний ​​зан чанар юм.`,
                E: `• Extroversion (E) - <b>Гадагшаа чиглэсэн, идэвхтэй хэв шинж</b>
                Өөрөөсөө гадна буюу хамт олны дунд байхаас сэтгэл ханамжийг эрэлхийлдэг төрлийн зан чанар юм.`,
                A: `• Agreeableness (A) – <b>Хүлцэнгүй хэв шинж</b>
                Өөрсдийн зан төлөвийг бусдад нийцүүлэн өөрчлөхийг илэрхийлнэ.`,
                N: `• Neuroticism (N) – <b>Тогтворгүй хэв шинж</b>
                Сэтгэл хөдлөлийн шинж чанартай холбоотой байдлыг илэрхийлнэ.`,
                 };

            const resultWindow = window.open("", "_blank");
        resultWindow.document.write(`
              <h1 style="color: #2c3e50;">Test Results</h1>
        <p style="color: #278c38;"><strong>Openness to Experience (O):</strong> ${O}</p>
        <p style="color: #c07d42;">${descriptions.O}</p>
        <p style="color: #e74c3c;"><strong>Conscientiousness (C):</strong> ${C}</p>
        <p style="color: #c0392b;">${descriptions.C}</p>
        <p style="color: #9b59b6;"><strong>Extroversion (E):</strong> ${E}</p>
        <p style="color: #8e44ad;">${descriptions.E}</p>
        <p style="color: #1abc9c;"><strong>Agreeableness (A):</strong> ${A}</p>
        <p style="color: #16a085;">${descriptions.A}</p>
        <p style="color: #f1c40f;"><strong>Neuroticism (N):</strong> ${N}</p>
        <p style="color: #f39c12;">${descriptions.N}</p>
        `);
        });
    </script>
</body>
</html>
