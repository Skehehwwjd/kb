<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8">
  <title>지역별 토너먼트 대진표</title>
  <style>
    body { font-family: 'Noto Sans KR', sans-serif; background: #f5f6fa; margin: 0; padding: 20px; }
    .container { max-width: 800px; margin: 0 auto; background: #fff; border-radius: 12px; box-shadow: 0 2px 8px #ddd; padding: 30px; }
    h1 { text-align: center; color: #333; margin-bottom: 30px; }
    .regions { display: grid; grid-template-columns: repeat(3, 1fr); gap: 20px; margin-bottom: 30px; }
    .region-box { border: 1px solid #ddd; padding: 15px; border-radius: 8px; }
    .region-box h3 { margin: 0 0 10px 0; color: #4e7cff; }
    textarea { width: 100%; height: 100px; padding: 8px; border: 1px solid #ccc; border-radius: 5px; resize: vertical; }
    button { display: block; margin: 20px auto; padding: 12px 40px; font-size: 1.1em; background: #4e7cff; color: #fff; border: none; border-radius: 5px; cursor: pointer; }
    .bracket { display: flex; justify-content: center; gap: 40px; margin-top: 30px; }
    .round { min-width: 200px; }
    .round-title { font-weight: bold; margin-bottom: 15px; color: #666; }
    .match { background: #f8f9ff; border: 1px solid #4e7cff; border-radius: 6px; padding: 12px; margin: 15px 0; text-align: center; }
    .bye { color: #999; font-style: italic; }
    @media (max-width: 768px) {
      .regions { grid-template-columns: 1fr; }
      .bracket { flex-direction: column; }
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>지역별 토너먼트 대진표 생성기</h1>
    
    <!-- 지역별 입력 영역 -->
    <div class="regions">
      <div class="region-box">
        <h3>지역 A</h3>
        <textarea id="regionA" placeholder="참가자 이름을 줄바꿈으로 입력"></textarea>
      </div>
      <div class="region-box">
        <h3>지역 B</h3>
        <textarea id="regionB" placeholder="참가자 이름을 줄바꿈으로 입력"></textarea>
      </div>
