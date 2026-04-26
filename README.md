# Database Design Workshop 4 - Relational Schema

## 项目简介
本项目基于 [Modern Database Management] 案例研究，完成了逻辑数据库设计。通过 EER 图建模、关系模式映射及 3NF 规范化处理，构建了包含客户、供应商、库存与员工职能的高效数据库架构。

## 核心设计点
- **规范化处理**：实现了 3NF 规范化，消除了部分依赖与传递依赖。
- **员工职能管理**：利用超级类型/子类型 (Supertype/Subtype) 处理了驱动程序、客服与会计的职能区分。
- **引用完整性**：定义了严谨的业务规则（Referential Integrity），确保数据一致性。

## 包含内容
- `workshop4_schema.sql`：完整的数据库定义脚本。
- `Relational_Schema_Design.pdf`：逻辑设计图纸与依赖分析。

## 运行环境
- Database: MySQL / SQL Server
