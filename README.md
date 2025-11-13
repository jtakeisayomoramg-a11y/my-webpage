<!DOCTYPE html>
<html lang="ja">
<head>
<meta charset="UTF-8" />
<title>じょーMコマ練できるかな？4桁コードでサイトオープン</title>
</head>
<body>
<h2>じょーMコマ練できるかな？問題を解いて4桁の数字を入力してください</h2>
<input type="password" id="codeInput" maxlength="4" pattern="\d{4}" placeholder="4桁の数字" />
<button onclick="checkCode()">開く</button>

<script>
function checkCode() {
  const input = document.getElementById('codeInput').value;
  const correctCode = "5651"; // ここに正しい4桁の数字をセット
  if (input === correctCode) {
    // 正解なら別ページに遷移する。下のURLを変更してください
    window.location.href = "https://docs.google.com/document/d/1Zi0R8CbLkPOzd4W_cYSurk7UG9-ECgK64ft-O2NJuhw/edit?usp=sharing";
  } else {
    alert("4桁の数字が違います。これじゃコマ練は始まんないよ");
  }
}
</script>
</body>
</html>
