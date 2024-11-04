<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tebakan Malam</title>
</head>
<body>
    <div id="text-container"></div>

    <script>
        const texts = [
            { text: "Hello, maleemm", delay: 2000 },
            { text: "Aku ada tebak-tebakkan nih", delay: 1000 },
            { text: "Kenapa kalau kerang ada di airrr?", delay: 1000 },
            { text: "Kenapa yaaa???", delay: 2000 },
            { text: "Karena kalau di darat nanti jadi keringg KWAWKAKWKW", delay: 1000 },
            { text: "Maaf ya garinggg, karena kalo melempem itu lupa nutup toples", delay: 1000 },
            { text: "Jiaaagghhh", delay: 1000 }
        ];

        let totalDelay = 0;
        texts.forEach(item => {
            totalDelay += item.delay;
            setTimeout(() => {
                const p = document.createElement("p");
                p.textContent = item.text;
                document.getElementById("text-container").appendChild(p);
            }, totalDelay);
        });
    </script>
</body>
</html>

