Sub 巨集1()
'
' 巨集1 巨集
'

'
Dim fId As Integer '若是巨量資料請設Long
Dim bCnt As Integer
bCnt = CInt(InputBox("請輸入目前內科廠區工作簿數量"))
For fId = 1 To bCnt

Workbooks.Open Filename:=ThisWorkbook.Path & "\內科" & fId & "廠.xlsx"

ActiveWorkbook.Sheets(1).Activate '第一張表啟動
'MsgBox ("此廠區資料共" & ActiveSheet.UsedRange.Rows.Count & "筆")
  
  '請將錄製好的巨集貼上在本行下方


ActiveWorkbook.Save
ActiveWorkbook.Close

Next

End Sub

