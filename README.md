<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>NeshNotes | Home</title>
<style>
body {
  margin: 0;
  font-family: "Segoe UI", Arial, sans-serif;
  background: #f5f7fa;
  color: #333;
}
#header {
  background: linear-gradient(135deg, #0f9d58, #0b8043);
  height: 90px;
  display: flex;
  align-items: center;
  padding: 0 25px;
  gap: 15px;
  color: white;
}
#header img {
  width: 55px;
  height: 55px;
  border-radius: 10px;
  flex-shrink: 0;
}
.title-wrapper {
  overflow: hidden;
  flex: 1;
}
.title-wrapper h1 {
  font-size: 28px;
  white-space: nowrap;
  animation: slideText 10s linear infinite;
}
@keyframes slideText {
  from { transform: translateX(100%); }
  to { transform: translateX(-100%); }
}
.about {
  max-width: 850px;
  margin: 90px auto 40px;
  background: #ffffff;
  padding: 40px;
  border-radius: 18px;
  box-shadow: 0 10px 30px rgba(0,0,0,0.08);
  opacity: 0;
  transform: translateY(35px);
  animation: aboutFade 3s ease forwards;
}
.about h3 {
  font-size: 26px;
  color: #0b8043;
  margin-bottom: 18px;
}
.about p {
  font-size: 15.5px;
  color: #555;
  line-height: 1.8;
  margin-bottom: 14px;
}
@keyframes aboutFade {
  from { opacity: 0; transform: translateY(45px); }
  to { opacity: 1; transform: translateY(0); }
}
