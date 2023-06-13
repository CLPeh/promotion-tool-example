# Create New Promotion Guideline

Before starting develop new promotion, please make sure you have read and understand all the information below:
- [README](../README.md)
- [Development Setup](dev-setup.md)
- [Architecture Design](architecture-design.md)
- [C# Coding Standards](https://www.dofactory.com/csharp-coding-standards)

### Steps
1. Create new promotion file in PromotionProcess.cs under ServiceProcessor.   
2. Add the code and replace the file name into the ServiceProcessor `ItemGroup` as below:  
    ```sh
    <Compile Update="NewPromotion.cs">
      <DependentUpon>PromotionProcess.cs</DependentUpon>
    </Compile>
    ```
3. Add necessary code into PromotionTypeExtensions as below with the promotion type to be created.
4. Add the new promotion type enum into PromotionType under Enums folder.
5. Start to code the promotion logic in the file created.
6. Do necessary unit testing to make sure the code is correct and workable.
