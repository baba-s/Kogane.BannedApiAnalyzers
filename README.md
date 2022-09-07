# Kogane Banned Api Analyzers

BannedApiAnalyzers を格納したパッケージ

## BannedSymbols.props の例

```xml
<Project xmlns="http://schemas.microsoft.com/developer/msbuild/2003">
    <ItemGroup>
      <Analyzer Include="Packages/com.baba-s.kogane-banned-api-analyzers/Editor/Microsoft.CodeAnalysis.BannedApiAnalyzers.dll" />
      <Analyzer Include="Packages/com.baba-s.kogane-banned-api-analyzers/Editor/Microsoft.CodeAnalysis.CSharp.BannedApiAnalyzers.dll" />
    </ItemGroup>
    <ItemGroup>
      <AdditionalFiles Include="$(ProjectDir)\BannedSymbols.txt" />
    </ItemGroup>
  </Project>
```

## BannedSymbols.txt の例

```
M:UnityEngine.Debug.Log(System.Object);Debug.Log は使用しないでください
```