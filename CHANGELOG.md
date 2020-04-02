# 更新日志

## 1.1.4 （2020.04.03）
- 升级 EPPlus 5+
  - .net: `appSettings` 增加 `<add key="EPPlus:ExcelPackage.LicenseContext" value="NonCommercial" />`
  - core: `appsettings.json` 根节点增加 `"EPPlus":{ "ExcelPackage":{ "LicenseContext":"NonCommercial" } }`
- 调整读取 Excel 方式


## 1.1.0 （2019.12.24）
- 移除 `LogHelper` ，转移到 `Rex.Helper.Core`，调整结构，减少依赖
- 增加 针对 `IEnumerable` 类型的 `IndexOf` 扩展
- 增加 单例类助手 `Singleton` 例：`public class ClassA : Singleton<ClassA>`
- 增加 `Distinct` 扩展更符合 Linq 一贯的风格 `var p1 = products.Distinct(p => p.ID);`
- 修改 `ResultModel` 命名空间 `System.GeneralExtensions.ResultModel`【和自己的其他项目有冲突了。。。】
