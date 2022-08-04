erAV0.11別人妊娠パッチ

妊娠発覚即臨月だったのでちょっと調整

EVENT_PREGNANCY.ERB内の213、224、235、247、259行目

CFLAG:TARGET:110 = DAY + 10 + RAND:3

に変更して出産まで10週+0～2に変更

EVENT_PREGNANCY.ERB内の287、297、308、319、329行目

&& CFLAG:COUNT:110 <= DAY+10

に変更して妊娠発覚時期を出産まで残り10週目に変更

EVENT_NEXTDAY.ERB内の96行目

IF (CFLAG:COUNT:110 - 2) == DAY

に変更して出産2週前に臨月状態に変更
となってるはず

おまけとして
VIDEO_TITLE.ERBの159行目より
CSTR:14判定内で妊娠中かどうかでタイトルが変化するように改造