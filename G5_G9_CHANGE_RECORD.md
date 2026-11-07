# G5/G9 产品修改记录

- 产品编号：$(@{number=77; product_id=JLZ-EDU-AG-016; chinese_name=教师能力发展; english_name=Teacher Development Agent; repository_name=edu-teacher-development-agent; repository_url=https://github.com/jinlize-tech/edu-teacher-development-agent; product_type=Agent; category_code=06; category=06 人力组织中心; description=教师能力诊断与发展规划。; target_users=System.Object[]; core_input=教师基本背景、课堂/教研证据、发展目标、任职阶段和可投入资源; main_output=能力诊断、差距、发展目标、90天成长计划、观察点和复盘机制; product_risk=把单次表现当能力定论或侵犯教师隐私; dedup_label=需要明确差异化; dedup_note=与教师成长反馈专家区分：本产品做个体发展计划编排；后者聚焦反馈机制；不复制完整教练平台。; development_status=Planned / 待研发; license=Apache-2.0; spec_version=1.0.0; workbuddy_status=PLANNED_FOR_WORKBUDDY}.product_id)
- 产品名称：教师能力发展
- 基线：EDUCATION_BASELINE_V1.0.0
- 基线提交：$BaselineCommit
- 原版本：1.0.0
- 新版本：1.0.1

## 本次修改

1. 强化产品专属执行流程、输入核对和输出验收规则。
2. 新增 scripts/validate_input.js，实际检查必填字段、冲突、未确认数据和敏感信息。
3. 新增正常、缺失、冲突、敏感信息和非法JSON场景输入。
4. 测试升级为 T1–T7 分层并保存逐项检查结果。
5. 安装包加入 Apache-2.0 LICENSE 和 THIRD_PARTY_NOTICES.md。
6. 安装包升级为 1.0.1，加入许可证、第三方声明和输入校验脚本，保留 1.0.0 ZIP。
7. 按本产品冻结规格补充专属处理规则、输入到成果的核对矩阵和去重边界。

## 产品专属增强

- 核心任务：教师能力诊断与发展规划。
- 主要风险：把单次表现当能力定论或侵犯教师隐私
- 去重边界：与教师成长反馈专家区分：本产品做个体发展计划编排；后者聚焦反馈机制；不复制完整教练平台。

- 从岗位任务、汇报关系、任职资格、协作接口和绩效证据出发，不针对个人画像。
- 区分必要条件与可培养条件，避免歧视性、无限扩张或不相关限制。
- 涉及劳动关系、纪律、薪酬和合规结论时要求专业人员复核。
- 招聘、培训、绩效和入职材料应保留责任人、时间与确认节点。

## 运行边界

- 本地模型行为：NOT_RUNTIME_VERIFIED
- WorkBuddy平台验证：WORKBUDDY_VALIDATION_NOT_IN_SCOPE
- 本轮不执行上传、安装、审核或正式发布。
