# Hi, names Daniil Rudenya

![Photo](Personal_Photo.jpg)

## [My Telegram](https://t.me/Daniil_Rudenya)

### My main goal is to get a job in a good company. My priorities are the team I work for, as well as the balance between my personal life and work. My strengths are stress tolerance, endurance, and efficiency. I am ready to learn new things and therefore at the moment I am studying at the university, studying Backend and Frontend development. 

### Stack: Git basics, C# basics, .NET basics, Delphi basics, Python basics, CSS and HTML basics.



# Code Examples
```Delphi
function AddingHashMethod(Value: int64; PacksAmount: integer): integer;
var
  StrNumber, MaxStr, First, Third, Right, Left: string;
  NumLen, PackageLen, MaxAmount, FirstPart, ThirdPart, SecondPart: int64;
begin
  // Преобразуем число в строку для удобства работы с цифрами
  while Length(IntToStr(Value)) > Length(IntToStr(PacksAmount)) do
  begin
    Right := '';
    Left := '';
    StrNumber := IntToStr(Value);
    NumLen := Length(StrNumber);
    // Вычисляем длину пакета
    PackageLen := NumLen - Length(IntToStr(PacksAmount));
    // Иначе вычисляем сумму первой и третьей частей
    First := Copy(StrNumber, 1, PackageLen div 2);
    if First <> '' then
      FirstPart := StrToInt(First)
    else
      FirstPart := 0;
    SecondPart := StrToInt(Copy(StrNumber, PackageLen div 2 + 1,
      Length(IntToStr(PacksAmount))));
    Third := Copy(StrNumber, Length(IntToStr(PacksAmount)) + PackageLen div 2 +
      1, PackageLen div 2 + PackageLen mod 2);
    if Third <> '' then
      ThirdPart := StrToInt(Third)
    else
      ThirdPart := 0;
    ThirdPart := ReverseNum(ThirdPart, Length(IntToStr(PacksAmount)));
    if Length(IntToStr(ThirdPart)) > Length(IntToStr(PacksAmount)) then
    begin
      Left := Copy(IntToStr(ThirdPart), 1, Length(IntToStr(PacksAmount)));
      Right := Copy(IntToStr(ThirdPart), Length(IntToStr(PacksAmount)) + 1,
        Length(IntToStr(ThirdPart)) - Length(IntToStr(PacksAmount)));
    end;
    if Left <> '' then
      ThirdPart := StrToInt(Left);
    Value := ReverseNum(FirstPart, Length(IntToStr(PacksAmount))) + SecondPart +
      ThirdPart;
    if Right <> '' then
      Value := StrToInt(IntToStr(Value) + Right);
  end;
  // Возвращаем сумму
  for var i := 1 to Length(IntToStr(PacksAmount)) do
    MaxStr := MaxStr + '9';
  MaxAmount := StrToInt(MaxStr);
  Result := Trunc(Value * ((PacksAmount - 1) / MaxAmount));
end;
```

## I took courses from Sololearn, ULearn.me , Stepik, etc. I am currently studying at the Belarusian State University of Informatics and Radioelectronics (BSUIR).


# English Level: B2
### Certificate
![Sertificate](EF%20SET%20Certificate.jpg)