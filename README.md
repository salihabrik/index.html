# index.html
<p align="left"> <img src=https://github.com/salihabrik/animated-profile-card#animated-profile-card
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Animated Profile Card</title>
    <link rel="stylesheet" href="style.css" />
</head>
<body>
    <div class="card">
        <div class="imgBx">
          <img src=""/>
        </div>
        <div class="content">
          <div class="details">
            <h2>salihabrik<br /><span>Frontend Developer</span></h2>
            <div class="data">
              <h3>26<br /><span>Posts</span></h3>
              <h3>2,106<br /><span>Followers</span></h3>
              <h3>90<br /><span>Following</span></h3>
            </div>
            <div class="actionBtn">
              <a href="https://twitter.com/SaLi46427585?" target="_blank">Follow</a>
              <a href="http://linkedin.com/in/salihabrik" target="_blank">connect</a>
            </div>
          </div>
        </div>
      </div>
</body>
</html>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Poppins", sans-serif;
}

body {
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;

  background: linear-gradient(
    109.6deg,
    rgb(150, 31, 23) 11.2%,
    rgb(16, 37, 60) 51.2%,
    rgb(0, 0, 0) 98.6%
  );
}

.card {
  position: relative;
  width: 350px;
  height: 190px;
  background: rgb(250, 250, 250);
  border-radius: 20px;
  box-shadow: 0 35px 80px rgba(0, 0, 0, 0.38);
  transition: 0.5s;
}

.card:hover {
  height: 350px;
  margin-top: 4rem;
}

.imgBx {
  position: absolute;
  left: 50%;
  top: -24%;
  transform: translateX(-50%);
  width: 136px;
  height: 136px;
  background: #fff;
  border-radius: 20px;
  box-shadow: 0 15px 50px rgba(0, 0, 0, 0.35);
  overflow: hidden;
  transition: 0.5s;
}

.card:hover .imgBx {
  width: 180px;
  height: 180px;
}

.imgBx img {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
}

/* ====================Content CSS============================== */

.card .content {
  position: absolute;
  width: 100%;
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: flex-end;
  overflow: hidden;
}

.card .content .details {
  padding: 40px;
  text-align: center;
  width: 100%;
  transition: 1s;
  transform: translateY(150px);
}

.card:hover .content .details {
  transform: translateY(0px);
}

.card .content .details h2 {
  font-size: 1.25em;
  font-weight: 600;
  color: rgba(34, 34, 34, 0.944);
  line-height: 1.2em;
}

.card .content .details h2 span {
  font-size: 0.75em;
  font-weight: 500;
  opacity: 0.5;
}

.card .content .details .data {
  display: flex;
  justify-content: space-between;
  margin: 20px 0;
}

.card .content .details .data h3 {
  font-size: 1em;
  color: rgb(49, 49, 49);
  line-height: 1.2em;
  font-weight: 600;
}

.card .content .details .data h3 span {
  font-size: 0.85em;
  font-weight: 400;
  opacity: 0.5;
}

.card .content .details .actionBtn {
  display: flex;
  justify-content: space-between;
}

.card .content .details .actionBtn a{
  padding: 10px 30px;
  border-radius: 5px;
  border: none;
  outline: none;
  font-size: 1em;
  font-weight: 500;
  background: #0092ca;
  color: #fff;
  cursor: pointer;
  transition: 0.3s;
  text-decoration: none;
}

.card .content .details .actionBtn a:hover {
  background: #00b3fa;
  color: #fff;
}

.card .content .details .actionBtn a:nth-child(2) {
  border: 1px solid #5c5c5c;
  color: #999;
  background: #fff;
  transition: 0.3s;
}

.card .content .details .actionBtn a:hover:nth-child(2) {
  color: rgb(255, 255, 255);
  background: #4f4f4f;
}
