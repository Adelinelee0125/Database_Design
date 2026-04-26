# Database Design Workshop 4 - Relational Schema

## 项目简介
本项目基于 [Modern Database Management] 案例研究，完成了逻辑数据库设计。通过 EER 图建模、关系模式映射及 3NF 规范化处理，构建了包含客户、供应商、库存与员工职能的高效数据库架构。

## 核心设计点
- **3NF 规范化处理**：通过分析功能依赖，消除了部分依赖 (Partial Dependency) 与传递依赖 (Transitive Dependency)，确保数据存储的原子性与无冗余。
- **员工职能层级化**：利用超级类型/子类型 (Supertype/Subtype) 结构，处理了驱动程序、客服与会计的特殊职能属性，确保数据结构的扩展性。
- **引用完整性 (RI) 保障**：定义了严谨的外键约束与业务规则，确保在增删改操作中系统的数据一致性。

## 技术挑战与解决方案
- **挑战**：如何处理多对多 (M:N) 库存关系以及员工角色的异构数据。
- **方案**：设计了 `INVENTORY` 关联实体以处理多对多映射，并采用 Disjoint (d) 约束处理员工超类/子类关系，有效降低了数据维护复杂度。

## 包含内容
- `workshop4_schema.sql`：完整的数据库定义脚本 (DDL)。
- `Relational_Schema_Design.pdf`：逻辑设计图纸、EER 建模分析与依赖关系图。

## 运行环境
- Database: MySQL 8.0 / SQL Server 2022+
