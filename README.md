# MsSqlToModelTemplate

> * Auto MsSql To Model Generater v2.0.0
> * (c) 2021-present Neil Hsieh
> * Released without License.

## 請修改以下5步驟，以利順利生成實體。

***
#### Step1：預設實體生成的位置會在 "資料夾MsSqlToModelTemplate" 的上一層，所以選擇將該資料夾放入要產生實體的位置即可。

***

#### Step2：MsSql 連接字符串設置。
string connectionString ="Data Source=127.0.0.1;Initial Catalog=northwind;User ID=sa;Password=sa;";

***

#### Step3：自定義你的命名空間。
var customNameSpace = "Example.Models";

***

#### Step4 : 刪除特定表。 （如果某些表不需要，則將這些表名添加到下面的字符串數組中。）
var withoutSpecficTableArray = new string[] { "NoNeedTable" };

***

#### Step5 : 只更新特定的表。 （如果您只需要特定表，則將這些表名添加到  onlyUpdateSpecficTableArray  的字符串數組中。）
#### 	警告：如果要更新“所有”表，“必須”讓 [onlyUpdateSpecficTableArray] 為空。
#### 	警告：如果要更新“所有”表，“必須”讓 [onlyUpdateSpecficTableArray] 為空。
#### 	警告：如果要更新“所有”表，“必須”讓 [onlyUpdateSpecficTableArray] 為空。
var onlyUpdateSpecficTableArray = new string[] { };

***

#### Step6：開始生成實體的兩種方式(目前環境是 VS2019)
#### 	方式1: 文件更新後保存。
#### 	方式2: 右擊“MsSqlToModel.tt”然後選擇[Debug T4 Template]就可以了。 

***