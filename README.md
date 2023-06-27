<!DOCTYPE html>
<html lang="en" xmlns="">
<head>
    <meta charset="UTF-8">
    <meta name="keywords" content="HTML & CSS">
    <meta name="description" content="Blog">
    <title>About Me</title>
    <link rel="stylesheet" href="css.css">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel='stylesheet' href='https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.1/css/all.min.css'>
    <link rel="stylesheet" href="css/style.css">
</head>
<body>
<div class="Container">
    <section id="About_Me">
        <div class="Text_Container">
            <div class="Animate_Animated Animate_Fade_In Title">About Me</div>
            <div class="Animate_Animated Animate_Zoom_In Animate_Delay_1s" id="Main_Text">Hi! Welcome!</div>
            <div id="Content_Text_About_Me"></div>
            <div> <img class="Picture" src="slika1.jpg" alt="Picture"></div>
            <div class="Buttons">
                <button class="Animate_Animated Animate_Fade_In"> <a href="projects.html">Projects</a></button>
                <button class="Animate_Animated Animate_Fade_In"> <a href="resume.html">Resume</a></button>
                <button class="Animate_Animated Animate_Fade_In"> <a href="contact.html">Contact</a></button>
            </div>
        </div>
    </section>
</div>
</body>
<script>
    let i = 0;
    const txt = 'Nice to meet you! My name is Andrej Ristovski and I am a coding and mathematics enthusiast. ' +
        'Currently I am studying Computer Science at the Faculty of Computer Science and Engineering in Skopje. ' +
        'Click on the buttons below to learn more about me.';
    const speed = 20;
    function typeWriter() {
        if (i < txt.length) {
            document.getElementById("Content_Text_About_Me").innerHTML += txt.charAt(i);
            i++;
            setTimeout(typeWriter, speed);
        }
    }
    typeWriter();
</script>
</html>
