휘경아

<span style="color:red;">이거봐봐</span>

진짜 신기하지 않니?

<!DOCTYPE html>
<html lang="ko">
<head>
<meta charset="UTF-8">
<title>Video Player</title>

<style>
body {
    font-family: Arial, sans-serif;
    display:flex;
    justify-content:center;
    align-items:center;
    height:100vh;
    background:#111;
}

#videoBox {
    position: relative;
    max-width: 720px;
    width:100%;
    cursor:pointer;
}

#videoBox img {
    width:100%;
    border-radius:12px;
}

.playBtn {
    position:absolute;
    top:50%;
    left:50%;
    transform:translate(-50%,-50%);
    font-size:70px;
    color:white;
    background:rgba(0,0,0,0.6);
    width:100px;
    height:100px;
    border-radius:50%;
    display:flex;
    justify-content:center;
    align-items:center;
}

iframe {
    width:100%;
    height:405px;
    border-radius:12px;
}
</style>
</head>

<body>

<div id="videoBox" onclick="playVideo()">
    <img src="https://img.youtube.com/vi/J5ofuLKjRDU/maxresdefault.jpg">
    <div class="playBtn">▶</div>
</div>

<script>
function playVideo() {
    document.getElementById("videoBox").innerHTML = `
    <iframe
        src="https://www.youtube.com/embed/J5ofuLKjRDU?autoplay=1"
        frameborder="0"
        allow="autoplay; encrypted-media"
        allowfullscreen>
    </iframe>`;
}
</script>


아빠가 영상도 이렇게 넣어서 웹페이지를 넣었어.

진수쟁이도 한번 봐바 신기하지?


</body>
</html>
