

## 🚀 **1. Real-World Project & Architecture Questions**

1. How would you structure Terraform code for a multi-environment setup (dev, stage, prod)?
2. What folder structure do you prefer in a large Terraform project?
3. How do you handle shared infrastructure like VPC or IAM roles used by multiple teams?
4. How do you manage Terraform modules across multiple repositories?
5. How would you create an EKS cluster and worker nodes using Terraform modules?
6. How do you pass VPC or subnet IDs dynamically between modules?
7. How do you handle Terraform state files in multi-account AWS setup?
8. What’s your approach for managing secrets (like DB passwords) in Terraform?
9. How do you use Terraform to manage networking (VPC, subnets, NAT gateways)?
10. How do you design Terraform workflows in Jenkins or GitHub Actions?
11. How do you roll out infrastructure changes safely in production?
12. How do you automate Terraform apply as part of CI/CD?
13. What strategies do you use to prevent accidental deletions of production resources?
14. How do you handle region-specific resource creation in a single Terraform project?
15. How do you scale your Terraform codebase as your infrastructure grows?

---

## 🧠 **2. State File Management (Most Asked in Real Interviews)**

16. What is the purpose of the Terraform state file?
17. What happens if your state file gets deleted or corrupted?
18. How do you recover from a lost Terraform state file?
19. How do you migrate a local state to a remote backend (e.g., S3)?
20. What’s the difference between local and remote state backends?
21. How do you configure state locking in Terraform?
22. What happens if two users run `terraform apply` at the same time?
23. How do you manage Terraform state in a team environment?
24. How do you split large state files for microservices or environments?
25. How do you inspect a state file to debug issues?
26. How can you remove a specific resource from the state file without destroying it?
27. What is `terraform state rm` used for?
28. When would you use `terraform state mv`?
29. What’s the difference between `terraform refresh` and `terraform plan`?
30. When does Terraform actually update the state file during apply?
31. How do you handle drift between state and actual infrastructure?
32. What are the risks of editing the state file manually?
33. How do you ensure state consistency in a CI/CD pipeline?

---

## 🧩 **3. Terraform Modules & Reusability**

34. How do you create reusable Terraform modules?
35. What’s the difference between a root module and a child module?
36. How do you version-control Terraform modules?
37. How do you pass outputs from one module to another?
38. How do you use Terraform registry modules securely?
39. How do you test your custom modules?
40. What are the pros/cons of using public vs private module registries?
41. How do you share modules across multiple teams?
42. How do you handle breaking changes in modules?
43. What is a good practice for naming variables and outputs in modules?
44. How do you handle cross-module dependencies?
45. How do you manage multiple providers in one module?
46. How do you use `for_each` with modules?
47. How do you use `count` and `for_each` together effectively?
48. When would you prefer a module over a resource block?

---

## 🧩 **4. Variables, Outputs & Locals**

49. How do you manage environment-specific variables?
50. What’s the purpose of locals?
51. How do you override variables from CLI or environment?
52. How do you securely pass secrets in variables?
53. How do you validate input variables?
54. What are sensitive variables in Terraform?
55. How do you use variable files like `dev.tfvars`?
56. How do you use dynamic blocks with variables?
57. When should you use outputs, and how do you use them across modules?
58. How do you hide outputs that contain secrets?
59. How do you reference outputs from one workspace to another?

---

## 🧩 **5. Workspaces (Multi-Environment Management)**

60. What is a Terraform workspace?
61. How do workspaces differ from using separate directories?
62. How do you manage environment-specific configurations using workspaces?
63. Can you use remote state with multiple workspaces?
64. What’s the naming convention for workspaces?
65. What happens to your state file when you create new workspaces?
66. When should you *not* use workspaces?

---

## ⚙️ **6. Terraform Execution Flow**

67. What happens internally when you run `terraform init`?
68. What happens during `terraform plan`?
69. When is the state file updated during `terraform apply`?
70. What happens if `terraform apply` fails midway?
71. What if you press `Ctrl + C` during `apply`?
72. How does Terraform handle dependencies between resources?
73. What happens if one resource fails during apply?
74. How does Terraform decide the order of resource creation?
75. How can you speed up Terraform apply for large infrastructures?
76. How do you handle retries or timeouts for slow API operations?

---

## 🧩 **7. Providers & Backends**

77. What is a provider in Terraform?
78. How do you configure multiple providers in one configuration?
79. How do provider versions affect your setup?
80. How do you use provider aliasing?
81. How do you authenticate providers (AWS, GCP, Azure)?
82. How do you handle provider credentials securely in CI/CD?
83. How do you pin provider versions to prevent breaking changes?
84. What is the difference between `backend` and `provider`?
85. How do you migrate from local backend to S3 backend safely?
86. What is a “partial configuration” in backend setup?

---

## 🧱 **8. Advanced Terraform Functions & Expressions**

87. What’s the difference between `count` and `for_each`?
88. How do you use `dynamic` blocks?
89. How do you use `lookup()` and `coalesce()` functions?
90. What are conditional expressions used for?
91. How do you handle optional variables?
92. How do you use `depends_on` properly in Terraform 1.x?
93. How do you use `concat`, `merge`, or `flatten` functions?
94. How do you use `locals` to simplify logic?
95. What is a “tainted” resource in Terraform?
96. How do you taint or untaint a resource manually?
97. How do you prevent Terraform from destroying a resource accidentally?
98. What’s the difference between `ignore_changes` and `lifecycle.prevent_destroy`?

---

## 🧩 **9. CI/CD Integration & Automation**

99. How do you integrate Terraform with Jenkins?
100. How do you handle Terraform backend credentials in Jenkins pipelines?
101. How do you validate Terraform code automatically in CI?
102. How do you run `terraform fmt` and `validate` as part of PR checks?
103. How do you handle concurrent Terraform applies in CI/CD?
104. How do you use workspaces in Jenkins?
105. How do you secure Terraform secrets in CI/CD pipelines?
106. How do you manage multiple environments in a pipeline?
107. What’s your strategy for rolling back failed infrastructure deployments?
108. How do you trigger a plan automatically on every PR?

---

## 🔐 **10. Security & Compliance**

109. How do you store and manage AWS credentials securely for Terraform?
110. How do you prevent sensitive data from being written to state files?
111. How do you encrypt Terraform state files in S3?
112. How do you handle Terraform secret rotation?
113. How do you integrate Terraform with HashiCorp Vault?
114. How do you enforce policies using Sentinel or OPA?
115. How do you restrict who can modify certain Terraform modules?

---

## 🧩 **11. Debugging & Troubleshooting**

116. How do you debug a stuck Terraform apply?
117. How do you increase log verbosity in Terraform?
118. What is the use of `TF_LOG` and `TF_LOG_PATH`?
119. How do you handle API rate limits in Terraform?
120. What’s the difference between a provider error and a configuration error?
121. How do you troubleshoot permission errors in Terraform apply?
122. How do you detect and fix resource drift?
123. What’s your strategy for handling intermittent API failures?

---

## 🧩 **12. Real-World Scenarios**

124. You have one VPC per environment — how do you ensure no cross-env resource overlap?
125. Your EC2 user data changes — how do you ensure Terraform re-runs it?
126. How do you handle blue-green deployments in Terraform?
127. How do you ensure consistent AMI IDs across environments?
128. How do you manage Terraform when AWS introduces new features?
129. How do you safely destroy an environment using Terraform?
130. You accidentally deleted a resource outside Terraform — what do you do?
131. How do you detect drift in production automatically?
132. How do you use `terraform import` in a live environment?
133. How do you handle version upgrades (e.g., Terraform 0.12 → 1.x)?

---

## 🧠 **13. Performance & Optimization**

134. How do you optimize Terraform for large deployments?
135. How do you manage provider rate limits?
136. What’s the impact of parallelism in Terraform?
137. How do you skip unchanged modules in large setups?
138. How do you clean up unused resources safely?

---

## ⚙️ **14. Advanced Concepts**

139. What is the difference between `plan` file (`.tfplan`) and state file?
140. How do you run Terraform in automation without manual approval?
141. How do you store `.tfplan` securely for audit?
142. How does Terraform ensure idempotency?
143. What is a data source and when should you use it?
144. How do you handle resources created outside Terraform (hybrid infra)?
145. What’s the role of the graph theory in Terraform’s execution engine?
146. What’s the difference between Terraform and CloudFormation conceptually?
147. How do you handle cross-cloud dependencies (AWS + Azure)?

---

## 🧩 **15. Enterprise & Team Practices**

148. How do you manage Terraform code for 50+ developers?
149. How do you enforce Terraform code quality?
150. How do you handle version control and PR approvals for Terraform changes?
151. How do you audit who made infrastructure changes?
152. How do you integrate Terraform with ServiceNow or ticketing tools?
153. How do you manage per-team IAM permissions for Terraform operations?
154. How do you organize Terraform for multi-account AWS structure (landing zone)?
155. What’s the difference between Terraform Cloud and Terraform Enterprise?
156. How do you use Terraform Cloud workspaces for collaboration?
157. How do you manage cost control using Terraform tagging?

---

## 🧩 **16. EKS-Specific & Cloud Infra Scenarios**

158. How do you provision an EKS cluster and node groups with Terraform?
159. How do you attach IAM roles to EKS service accounts via Terraform?
160. How do you configure aws-auth configmap post-EKS creation?
161. How do you manage kubeconfig generation with Terraform?
162. How do you integrate Terraform EKS provisioning with ArgoCD or Helm?
163. How do you use Terraform to deploy Kubernetes resources (via `kubernetes` provider)?
164. How do you handle multiple EKS clusters with same Terraform code?

---

## 🧩 **17. Misc Advanced & Real-Life Recovery**

165. What’s the safest way to rollback a bad Terraform apply?
166. How do you re-create a single resource without touching others?
167. How do you handle partial apply failures in production?
168. What is Terraform drift detection strategy for large teams?
169. How do you rotate IAM access keys without downtime using Terraform?
170. How do you move resources from one state file to another?
171. How do you combine Terraform with Ansible or Helm in workflows?

---

## 🔥 **18. Deep-Dive Expert Questions (Terraform Internals)**

172. Explain Terraform’s DAG (Directed Acyclic Graph) execution model.
173. What is provider schema?
174. What happens internally when Terraform refreshes the state?
175. What is resource addressing in Terraform (e.g., `aws_instance.web[0]`)?
176. How does Terraform handle parallelism and dependency ordering?
177. What is Terraform’s difference between desired vs current vs planned state?
178. What are Terraform provisioners, and why are they discouraged?
179. How does Terraform detect drift without state refresh?
180. How is Terraform idempotent by design?
181. How do you debug dependency cycles?
182. What is Terraform plan file serialization format?

---

## 🧩 **19. Terraform + Vault / Secrets / Integration**

183. How do you fetch secrets from HashiCorp Vault in Terraform?
184. How do you prevent secrets from appearing in plan logs?
185. How do you use Vault provider vs external data source for secrets?
186. How do you rotate secrets automatically with Terraform?
187. How do you inject dynamic credentials (DB, AWS) at runtime?

---

## 🧩 **20. Terraform + GitHub / GitOps**

188. How do you trigger Terraform runs via GitHub Actions?
189. How do you approve Terraform apply in GitHub PR workflow?
190. How do you store Terraform plan artifacts in GitHub Actions?
191. How do you use Atlantis for Terraform automation?
192. How do you use Terraform in a GitOps setup with ArgoCD?

---

## 🧩 **21. Error Handling Scenarios**

193. What happens when a dependent resource fails to create?
194. How do you retry transient API errors automatically?
195. How do you ensure cleanup after partial failure?
196. How do you fix “Resource already exists” errors?
197. How do you fix “Resource not found” errors after manual deletion?
198. How do you deal with Terraform provider version mismatch errors?
199. How do you handle long-running Terraform operations?

---

## 🧩 **22. Terraform Best Practices**

200. How do you organize Terraform for readability and maintainability?
201. How do you document Terraform modules?
202. How do you ensure reproducible builds?
203. How do you manage provider version upgrades?
204. How do you secure Terraform pipelines?
205. How do you monitor Terraform operations?
206. How do you enforce tagging policies via code?
207. How do you review Terraform changes in PRs?
208. How do you perform drift detection as part of CI/CD?
209. How do you manage cost estimation before apply?

---

## 🧩 **23. Multi-Cloud & Cross-Integration**

210. How do you use Terraform to deploy resources in multiple clouds simultaneously?
211. How do you manage different credentials for AWS and GCP in one codebase?
212. How do you build hybrid-cloud networking using Terraform?
213. How do you avoid hardcoding provider credentials across clouds?
214. How do you handle naming conventions across providers?

---

## 🧩 **24. Disaster Recovery & Rollback**

215. How do you recover a lost or corrupted state file?
216. How do you back up Terraform state automatically?
217. How do you roll back Terraform apply safely?
218. What’s your DR strategy for Terraform-managed infrastructure?
219. How do you restore infrastructure if an apply accidentally deletes something?

---

## 🧩 **25. Terraform Cloud / Enterprise**

220. What advantages does Terraform Cloud provide over local runs?
221. How do you manage user access and policies in Terraform Cloud?
222. How do you set up Terraform Cloud workspaces per environment?
223. How do you connect Terraform Cloud to GitHub repos?
224. How do you handle Terraform Cloud variable sets and secrets?
225. What’s the difference between remote execution and local execution in Terraform Cloud?
226. How do you enforce Sentinel policies in Terraform Cloud?

---

## 🧩 **26. Terraform Upgrades / Maintenance**

227. How do you upgrade Terraform from 0.12 to 1.x?
228. What is `terraform 0.12upgrade` used for?
229. How do you manage provider version updates?
230. How do you test Terraform version upgrades safely?
231. How do you handle deprecated resources or attributes?

---

## 🧩 **27. Real Enterprise Challenges**

232. How do you handle 100+ developers using Terraform across multiple teams?
233. How do you manage different cloud accounts securely?
234. How do you monitor who changed what infrastructure when?
235. How do you enforce change approvals in Terraform?
236. How do you manage cross-region infrastructure replication?
237. How do you ensure Terraform changes are auditable?
238. How do you standardize modules across teams?
239. How do you ensure zero downtime infrastructure updates?
240. How do you handle API throttling in large Terraform runs?

---

## 🧩 **28. Terraform with Networking**

241. How do you create multi-AZ subnets with Terraform dynamically?
242. How do you ensure correct CIDR allocation automatically?
243. How do you attach route tables and gateways dynamically?
244. How do you ensure private/public subnets get correct routes?
245. How do you handle IP conflicts or changes in Terraform-managed networks?

---

## 🧩 **29. Terraform + Monitoring**

246. How do you integrate Terraform with Prometheus/Grafana for infra metrics?
247. How do you export Terraform output values to monitoring tools?
248. How do you alert on failed Terraform runs?
249. How do you audit Terraform state changes over time?
250. How do you use cost estimation tools like Infracost with Terraform?


=================================================================================================================================

REAL-WORLD TERRAFORM QUESTIONS (1–25)
=====================================

1. Multi-environment setup
--------------------------
Use separate states and modules. Reuse code via `modules/`, and have env-specific configs in `environments/dev|stage|prod`. Each env uses its own backend and vars. Promote changes via CI/CD.

2. Preferred folder structure
-----------------------------
/modules/ (reusable units)
 /environments/dev|stage|prod (root configs)
 /global/ (shared infra)
 /README.md /ci.yml
Keep modules atomic; root just connects them.

3. Shared infrastructure
------------------------
Deploy shared VPC/IAM once in a separate account/state. Expose via module outputs or remote state. Consumer teams reference via data sources.

4. Managing modules across repos
--------------------------------
Use a private module registry or Git with version tags. Reference with source URLs + ref tag. Use CI to release versions.

5. EKS cluster setup
--------------------
Create `modules/eks` + `modules/nodegroup`. Root passes VPC/IAM vars. Use `aws_eks_cluster`, `aws_eks_node_group`, automate aws-auth.

6. Pass VPC/subnet IDs dynamically
----------------------------------
Use module outputs (`module.vpc.subnet_ids`) passed to other modules or via `terraform_remote_state`.

7. Multi-account AWS state handling
-----------------------------------
Use per-account/per-env S3 backend + DynamoDB locking. Encrypt state, restrict IAM access, unique state keys per env.

8. Secrets management
---------------------
Never hardcode. Use Vault/AWS Secrets Manager, mark vars as `sensitive`, avoid secrets in outputs/logs, use secure CI secrets.

9. Networking via Terraform
---------------------------
Use a `vpc` module (VPC, subnets, IGW, NAT). Parameterize CIDRs/AZs. Use `for_each` for subnets and tag all resources.

10. CI/CD workflows (Jenkins/GitHub)
------------------------------------
Run fmt/validate/plan on PR. Store plan artifact. Require approval before prod apply. Use role-assume for CI auth.

11. Safe production rollouts
----------------------------
Use canary/blue-green, review plan, small changes. Protect critical resources with `prevent_destroy`, have rollback plan.

12. Automate apply
------------------
Automate for dev/stage only. For prod, use manual approval. Use CI job with assumed role and gated apply stage.

13. Prevent accidental deletions
-------------------------------
Use `lifecycle { prevent_destroy = true }`, CI approvals, RBAC restrictions, and Sentinel/OPA policies. Backup states.

14. Region-specific resources
-----------------------------
Use provider aliases or per-region configs. Parameterize region vars. For complex setups, separate region folders.

15. Scaling Terraform codebase
------------------------------
Modularize, split state per domain/env, version modules, lint/test via Terratest, enforce code review + policy checks.

16. Purpose of state file
-------------------------
Maps Terraform resources to real ones; tracks metadata and dependencies. Enables planning and updates.

17. If state file deleted/corrupted
-----------------------------------
Terraform loses mapping → risks re-creation or deletion. Restore from backup or import resources to rebuild.

18. Recover lost state
----------------------
Restore from backups (S3 versioning). If missing, `terraform import` each resource, or rebuild infra manually.

19. Migrate local → remote backend
----------------------------------
Edit backend config, run `terraform init`, confirm migration, enable locking (DynamoDB). Verify after migration.

20. Local vs remote backend
---------------------------
Local = stored on disk (solo use). Remote = shared, supports locking, versioning, IAM control (team safe).

21. Configure state locking
---------------------------
For S3: use DynamoDB table via `dynamodb_table` backend config. Terraform Cloud handles locking automatically.

22. Two users run apply simultaneously
--------------------------------------
With locking: one waits/fails until unlocked. Without locking: risk of corruption/conflicts.

23. State management in teams
-----------------------------
Use remote backend + locking. Restrict permissions. CI applies only. Version S3. Avoid local applies.

24. Split large state files
---------------------------
Divide by domain/env (networking, app, db). Separate Terraform roots/states. Reduce blast radius.

25. Inspect state file
----------------------
Use `terraform state list` and `terraform state show`. Pull remote with `terraform state pull`. Avoid manual edits; use subcommands safely.

REAL-WORLD TERRAFORM QUESTIONS (26–50)
======================================

🧱 ADVANCED STATE & WORKSPACES
------------------------------

26. Remove resource from state (without deleting)
-------------------------------------------------
Use: terraform state rm <resource_address>
Removes from state only; resource stays in cloud.

27. Import existing resource into state
---------------------------------------
Use: terraform import <resource_address> <cloud_resource_id>
Example: terraform import aws_instance.web i-0123abcd
Then run plan to confirm match.

28. Handle state drift
----------------------
Run terraform plan to detect drift or terraform plan -refresh-only to check without changes.

29. View remote backend state
-----------------------------
Use: terraform state pull > state.json
Inspect via jq, avoid manual edits.

30. Fix corrupted state
-----------------------
1. Pull latest remote copy.
2. Restore from backup/versioning.
3. Re-import resources if needed.
4. Avoid manual JSON edits.

31. Use of workspaces
---------------------
Workspaces isolate state for same config (dev, stage, prod). Useful for simple envs or multi-tenant setups.

32. Create & switch workspaces
------------------------------
terraform workspace new dev  
terraform workspace list  
terraform workspace select prod

33. Why not use workspaces for prod envs
----------------------------------------
They share backend and IAM context; risk of misapply. Prefer separate states/repos per environment.

34. Migrate state between backends
----------------------------------
Edit backend config or run: terraform init -migrate-state
Copies state to new backend (e.g., local → S3).

35. Difference between refresh & plan
-------------------------------------
refresh = update state only  
plan = compare refreshed state vs config to show diffs

🔐 VARIABLES & SECRETS
----------------------

36. Organize variables
----------------------
variables.tf → definitions  
terraform.tfvars → defaults  
<env>.tfvars → env-specific  
secrets.auto.tfvars → sensitive, not in Git

37. Provide variable values
---------------------------
.tfvars files, -var/-var-file flags, TF_VAR_ env vars, Terraform Cloud vars, CI secrets.

38. Handle sensitive variables
------------------------------
Mark variable with sensitive = true; hide from output/logs. Use Vault or Secrets Manager for storage.

39. Use env vars as inputs
--------------------------
Prefix with TF_VAR_.  
Example: export TF_VAR_region=us-east-1

40. terraform.tfvars vs .auto.tfvars
------------------------------------
Both auto-loaded. .auto.tfvars allows grouped sets. Override via -var-file.

41. Dynamically generate vars
-----------------------------
Use locals/data sources:  
locals { private_subnets = [for s in data.aws_subnets.private.ids : s] }

42. Fetch secrets from AWS Secrets Manager
------------------------------------------
data "aws_secretsmanager_secret_version" "db" {
  secret_id = "my-db-password"
}
Use data.aws_secretsmanager_secret_version.db.secret_string

43. Fetch secrets from Vault
----------------------------
data "vault_generic_secret" "db" {
  path = "secret/data/prod/db"
}
Use data.vault_generic_secret.db.data["password"]

44. Inject external script data
-------------------------------
data "external" "example" {
  program = ["python3", "${path.module}/script.py"]
}
Script must return JSON output.

45. Interpolate maps/lists
--------------------------
variable "users" { type = map(string) }
output "emails" { value = [for n,e in var.users : "${n} <${e}>"] }

⚙️ EXECUTION & PLAN DETAILS
---------------------------

46. Purpose of .terraform.lock.hcl
----------------------------------
Locks provider versions for consistent builds. Checked into Git, updated via terraform init -upgrade.

47. Upgrade providers safely
----------------------------
Run terraform init -upgrade then plan. Review changes and pin versions as needed.

48. apply vs apply planfile
---------------------------
apply = immediate plan+apply  
apply planfile = uses saved plan for consistent results (CI-safe).

49. Handle partial resource failures
------------------------------------
Failed resources marked tainted; recreated on next run.
Manual: terraform taint/un-taint <resource>.

50. Debug apply issues
----------------------
Use TF_LOG=DEBUG, check provider versions, disable refresh with plan -refresh=false, and isolate modules for testing.

REAL-WORLD TERRAFORM QUESTIONS (51–75)
======================================

🧩 MODULES & REUSABILITY
------------------------

51. Why use Terraform modules
-----------------------------
Modules enable code reuse, consistency, and clean architecture.
Encapsulate infra logic (like VPC, EKS) once, reuse via inputs/outputs.

52. Root vs Child module
------------------------
Root = main directory where Terraform runs.
Child = module called via source (local, Git, registry).
Example: module "vpc" { source = "../modules/vpc" }

53. Pass outputs between modules
--------------------------------
Module A:
  output "vpc_id" { value = aws_vpc.main.id }
Module B:
  vpc_id = module.vpc.vpc_id
Use terraform_remote_state for cross-state sharing.

54. Version control for modules
-------------------------------
Use semantic versioning and Git tags (v1.0.0).
Reference via source = "git::ssh://...ref=v1.0.0" for reproducibility.

55. Test modules before prod
----------------------------
Use Terratest, tflint, tfsec in CI.
Run fmt, validate, plan in sandbox. Destroy after verification.

56. Publish private modules
---------------------------
Repo naming: terraform-<PROVIDER>-<NAME>.
Publish via Terraform Cloud “Modules” → “Publish”.
Restrict access via org/team permissions.

57. Share outputs across workspaces
-----------------------------------
Use terraform_remote_state:
data "terraform_remote_state" "network" {
  backend = "s3"
  config = {
    bucket = "tf-state"
    key    = "network/prod.tfstate"
    region = "us-east-1"
  }
}

58. count vs for_each
---------------------
count = list, numeric index  
for_each = map/set, named keys  
for_each gives stable addressing when order changes.

59. Make module env-agnostic
----------------------------
Parameterize all env-specific data via variables (CIDR, tags, names).
Inject via .tfvars at root level.

60. Share module across repos
-----------------------------
Use Git source with tagged versions or private registry (Terraform Cloud, Artifactory).
Automate version release via CI.

⚙️ PROVISIONERS, LIFECYCLE & HOOKS
----------------------------------

61. What are provisioners
-------------------------
local-exec / remote-exec run scripts post resource creation.
Use only if provider lacks native setup (prefer userdata or Ansible).

62. local-exec vs remote-exec
-----------------------------
local-exec = runs on Terraform host  
remote-exec = runs inside instance (SSH/WinRM)

63. null_resource usage
-----------------------
Used for orchestration or triggers without infra.
resource "null_resource" "example" {
  triggers = { build = timestamp() }
  provisioner "local-exec" { command = "echo Deploying..." }
}

64. lifecycle block
-------------------
Controls Terraform behavior:
prevent_destroy, ignore_changes, create_before_destroy.

65. ignore_changes usage
------------------------
Skips attributes modified outside Terraform (e.g., autoscaling desired_capacity).

66. create_before_destroy usage
-------------------------------
Ensures zero-downtime by creating new resource before destroying old (ALB, IAM roles).

67. Tainted resource
--------------------
Resource flagged for recreation due to failure/corruption.
Recreated on next apply. Manual: terraform taint <resource>.

68. Fix tainted resource
------------------------
If healthy: terraform untaint <resource>.
If broken: allow apply to recreate or delete manually first.

69. Handle transient apply errors
---------------------------------
Use provider retries, backoff, and smaller apply batches.
Re-run terraform apply safely; state ensures idempotency.

70. Debug provisioner failures
------------------------------
Use TF_LOG=DEBUG, check SSH connections, on_failure=continue, capture logs to files.

🧠 ERROR HANDLING & SECURITY
----------------------------

71. Secure state files
----------------------
Use remote encrypted backend (S3+KMS, Terraform Cloud).
Restrict IAM access, enable locking & versioning. Never output secrets.

72. Prevent secret leaks in logs
-------------------------------
Mark variables/outputs sensitive=true.
Filter CI logs, avoid echoing secrets, use Vault for tokens.

73. Audit infra changes
-----------------------
Enable S3 versioning, commit configs to Git, use Terraform Cloud run history, and store plan files.

74. Restrict who can apply
--------------------------
Use IAM least-privilege roles, CI-controlled apply, Terraform Cloud RBAC, and policy-as-code (Sentinel/OPA).

75. Manage credentials securely
-------------------------------
Use STS/Vault temporary tokens, no static keys in CI/local.
Store in secret managers and use IAM roles for access.


TERRAFORM INTERVIEW QUESTIONS (76–100)
======================================

☁️ BACKENDS, STATE & DRIFT (Q76–85)
-----------------------------------

76. What is a backend & why used?
→ Defines where/how Terraform stores state & performs operations.
→ Enables collaboration, locking, remote storage.
→ Examples: local, s3, azurerm, gcs, terraform cloud.

77. Difference: local vs remote backend
| Type | Storage | Collaboration | Locking |
| local | Local disk (tfstate) | No | No |
| remote | S3 / TFC | Yes | Yes (DynamoDB/TFC) |
→ Remote backend avoids state overwrites in team setups.

78. Configure S3 backend with locking:
  terraform {
    backend "s3" {
      bucket         = "tf-state-prod"
      key            = "network/terraform.tfstate"
      region         = "us-east-1"
      dynamodb_table = "terraform-lock"
      encrypt        = true
    }
  }
→ S3 = state, DynamoDB = locking, encrypt=true for SSE.

79. State file deleted accidentally?
→ Terraform loses infra tracking.
→ Fix:
  - Use terraform import to rebuild state.
  - Restore from S3 versioning backup.
→ Always enable versioning + lock table.

80. What is drift?
→ Infra differs from expected state (manual changes, failed applies).
→ Detected during terraform plan.

81. Detect & fix drift:
→ Run terraform plan.
→ Fix by:
  - terraform apply (to correct)
  - or update configs to match console.

82. Refresh state manually:
→ terraform refresh
→ Syncs state w/ real infra (deprecated 1.6+, use plan instead).

83. Migrate local → remote backend:
→ Add backend block, then:
  terraform init -migrate-state
→ Safely moves local state to remote.

84. Two applies at once?
→ Not allowed when locking enabled.
→ Error: “Error acquiring state lock”
→ Prevents corruption.

85. Handle partial/failed creates:
→ Terraform tracks created resources.
→ Inspect .tfstate / refresh / rerun apply.
→ Taint or import if broken.

-----------------------------------

🔍 DATA SOURCES, IMPORTS & DEPENDENCIES (Q86–90)
-----------------------------------

86. What is a data source?
→ Reads info from existing infra (no creation).
Example:
  data "aws_ami" "latest" {
    most_recent = true
    owners      = ["amazon"]
    filters = [{ name="name", values=["amzn2-ami-hvm-*"] }]
  }

87. Data source vs resource:
| Type | Behavior |
| resource | Creates infra |
| data | Reads existing |
→ resource = build, data = reference.

88. Import existing resource:
→ terraform import aws_instance.example i-12345
→ Define resource manually in .tf file.
→ Adds to state but not config.

89. Auto-generate config after import:
→ terraform plan -generate-config-out=generated.tf
→ (Terraform 1.6+)
→ Writes discovered config to file.

90. Manage dependencies:
→ Implicit via references:
    subnet_id = aws_subnet.main.id
→ Explicit via depends_on = [aws_vpc.main]

-----------------------------------

☁️ TERRAFORM CLOUD & ENTERPRISE (Q91–95)
-----------------------------------

91. Benefits of Terraform Cloud:
→ Central backend, RBAC, audit logs
→ VCS integration, Sentinel policies, run history, cost estimation.

92. How Terraform Cloud runs:
→ CLI uploads config → remote workers execute securely using stored creds.

93. Trigger TFC runs:
→ VCS push/PR → auto plan/apply.
→ Or via terraform apply -remote or API/webhooks.

94. What is Sentinel?
→ Policy-as-Code engine for compliance.
→ Example rule:
  aws_instance_type == "t3.micro"
→ Enforce tagging, region, size, cost policies.

95. Cloud vs Enterprise:
| Feature | Cloud | Enterprise |
| Hosting | SaaS | Self-hosted |
| Cost | Free/Paid | Enterprise license |
| Integrations | Limited | Full, private registry, SSO |

-----------------------------------

🧠 CI/CD & TROUBLESHOOTING (Q96–100)
-----------------------------------

96. CI/CD Integration (Jenkins/GitHub Actions):
→ Steps:
  1. terraform fmt, validate, plan
  2. Save plan artifact
  3. Manual/PR approval
  4. terraform apply (from plan)
→ Use Vault or roles for creds.

97. Error acquiring state lock:
→ Check DynamoDB table exists.
→ Remove stale lock:
  terraform force-unlock <LOCK_ID>
→ Don’t run parallel applies.

98. Plan shows “destroy” unexpectedly:
→ Causes: drift, missing resource, state corruption.
→ Fix: verify resource → import again → rerun plan.

99. Provider rate limit (API throttling):
→ Add timeouts, reduce parallelism (-parallelism=1)
→ Retry/backoff (auto in TF)
→ Split infra by region/module.

100. Rollback failed changes:
→ No direct rollback in Terraform.
→ Options:
  - Restore previous state (S3 version)
  - Git revert → reapply
  - terraform destroy & redeploy cleanly.

TERRAFORM ADVANCED TOPICS (Q101–125)
====================================

🌍 MULTI-ENVIRONMENT SETUP & BEST PRACTICES
-------------------------------------------

101. Ways to manage multiple environments:
- Workspaces (dev, qa, prod)
- Separate directories/repositories
- Single module + multiple .tfvars
- Terraform Cloud workspaces per env

102. Pros & Cons of Workspaces:
+ Easy switching, single config base
- Hard to isolate state & creds
→ Best for small/non-prod setups

103. Directory Structure Example:
modules/
 ├─ vpc/
 ├─ eks/
 └─ rds/
environments/
 ├─ dev/
 ├─ stage/
 └─ prod/

104. Backend per environment:
terraform init \
  -backend-config="bucket=my-tfstate-prod" \
  -backend-config="key=prod/terraform.tfstate"

105. Isolating dev & prod:
- Separate AWS accounts & IAM roles
- Different backend buckets
- Restrict CI/CD access by IAM

106. Reusable variable files:
terraform apply -var-file=common.tfvars -var-file=prod.tfvars

107. Env-specific naming:
name = "${var.env}-vpc"

108. Workspaces vs State files:
| Concept | Workspace | State file |
|----------|------------|------------|
| Backend | Shared | Separate |
| Access | Shared creds | Isolated |
| Use case | Small setup | Large/prod |

109. Avoid hardcoding:
- Use data sources
- Use SSM/Vault/locals.tf for lookup

110. Multi-region/account:
provider "aws" { alias="us_east_1" region="us-east-1" }
resource "aws_instance" "east" { provider = aws.us_east_1 }

🔐 SECRET MANAGEMENT & VAULT INTEGRATION
---------------------------------------

111. Storing secrets safely:
- Use Vault/Secrets Manager/SSM
- data "vault_generic_secret" "db" { path="secret/data/db-creds" }

112. Injecting secrets in CI/CD:
- Jenkins fetches from Vault API
- Exports TF_VAR_ variables
- Use sensitive = true

113. Prevent secrets in plan/logs:
- sensitive = true
- No outputs
- Dynamic secrets
- Auto-approve in CI

114. Vault dynamic secrets:
- Ephemeral, auto-expire
- Safer for pipeline creds
- Runtime fetch reduces leaks

115. Secret rotation:
- Vault auto-rotate policies
- terraform taint + apply
- Sync via external scripts

⚙️ CI/CD INTEGRATION & AUTOMATION
---------------------------------

116. Jenkins Terraform flow:
1. terraform fmt
2. terraform validate
3. terraform plan (store artifact)
4. Approval
5. terraform apply

117. Plan approvals:
- Jenkins input step / PR review
- Apply stored plan file after approval

118. Multi-env in Jenkins:
if (params.ENV == 'prod') {
  dir('environments/prod') {
    sh 'terraform apply'
  }
}

119. State backend credentials:
- Use Jenkins credentials or Vault plugin
- Assume IAM roles via aws sts assume-role

120. Rollback automation:
- Restore previous S3 version
- Apply old .tfvars
- Re-deploy for non-prod

🏗️ SCALING, PERFORMANCE & LARGE INFRA
-------------------------------------

121. Speed up large applies:
- terraform apply -parallelism=10
- Split infra into modules
- Parallel pipelines
- Cache lookups

122. Managing 100+ modules:
- Use internal module registry
- Enforce naming/tagging
- Version pinning
- Separate states per domain

123. Consistent tagging:
locals {
  common_tags = {
    Owner = "DevOps"
    Env = var.env
    ManagedBy = "Terraform"
  }
}
tags = local.common_tags

124. Multi-account authentication:
provider "aws" {
  alias  = "dev"
  region = "us-east-1"
  profile = "dev"
}
→ In CI: assume roles per env

125. Concurrency control:
- Remote backend + DynamoDB locking
- Separate states per env
- CI job queueing
- Plan preview → approved apply


TERRAFORM WITH AWS (Q126–150)
=============================

☁️ AWS INFRASTRUCTURE AS CODE (Q126–135)
----------------------------------------

126. Create AWS VPC
-------------------
resource "aws_vpc" "main" {
  cidr_block = "10.0.0.0/16"
  enable_dns_support   = true
  enable_dns_hostnames = true
  tags = { Name = "main-vpc" }
}
→ Modularize using modules/vpc for cleaner structure.

127. Associate multiple subnets to route table
----------------------------------------------
resource "aws_route_table_association" "subnets" {
  for_each = toset(var.subnet_ids)
  subnet_id      = each.value
  route_table_id = aws_route_table.main.id
}

128. Create multiple security groups dynamically
------------------------------------------------
resource "aws_security_group" "sg" {
  for_each = var.sg_rules
  name        = each.key
  description = each.value.desc
  vpc_id      = aws_vpc.main.id
}

129. Handle dependencies
------------------------
Terraform auto-detects via references.
Manual control: depends_on = [aws_vpc.main]

130. Manage multiple regions
----------------------------
provider "aws" { alias = "east" region = "us-east-1" }
provider "aws" { alias = "west" region = "us-west-2" }
resource "aws_instance" "web" { provider = aws.east }

131. Manage multiple accounts
-----------------------------
Use separate backends and assume_role:
provider "aws" {
  assume_role { role_arn = var.role_arn }
}

132. Create EC2 dynamically
---------------------------
variable "servers" { default = ["app1","app2","app3"] }
resource "aws_instance" "ec2" {
  for_each = toset(var.servers)
  ami = var.ami
  instance_type = "t3.micro"
  tags = { Name = each.key }
}

133. Attach IAM role to EC2
---------------------------
resource "aws_iam_role" "ec2_role" {
  assume_role_policy = data.aws_iam_policy_document.assume.json
}
resource "aws_iam_instance_profile" "profile" {
  role = aws_iam_role.ec2_role.name
}
resource "aws_instance" "server" {
  iam_instance_profile = aws_iam_instance_profile.profile.name
}

134. Use user data
------------------
resource "aws_instance" "web" {
  ami = var.ami
  instance_type = "t2.micro"
  user_data = file("userdata.sh")
}

135. Attach existing EBS volume
-------------------------------
resource "aws_volume_attachment" "ebs_att" {
  device_name = "/dev/sdh"
  volume_id   = aws_ebs_volume.data.id
  instance_id = aws_instance.web.id
}

🧩 EKS & KUBERNETES (Q136–145)
-------------------------------

136. Provision EKS
------------------
module "eks" {
  source = "terraform-aws-modules/eks/aws"
  cluster_name = "prod-eks"
  cluster_version = "1.29"
  vpc_id = aws_vpc.main.id
  subnet_ids = aws_subnet.eks[*].id
}

137. Authenticate kubectl
-------------------------
aws eks update-kubeconfig --name <cluster-name> --region <region>

138. Manage EKS worker nodes
----------------------------
module "eks_node_group" {
  source = "terraform-aws-modules/eks/aws//modules/node_groups"
  cluster_name = module.eks.cluster_name
  node_groups = {
    general = { desired_capacity = 2, max_capacity = 4 }
  }
}

139. Configure EKS add-on
-------------------------
resource "aws_eks_addon" "cni" {
  cluster_name = module.eks.cluster_name
  addon_name = "vpc-cni"
  resolve_conflicts = "OVERWRITE"
}

140. Manage K8s manifests via provider
-------------------------------------
provider "kubernetes" {
  host = module.eks.cluster_endpoint
  cluster_ca_certificate = base64decode(module.eks.cluster_certificate_authority_data)
  token = data.aws_eks_cluster_auth.main.token
}
resource "kubernetes_namespace" "dev" {
  metadata { name = "dev" }
}

141. Wait for EKS before K8s apply
----------------------------------
depends_on = [module.eks]

142. Manage Helm charts
-----------------------
resource "helm_release" "nginx" {
  name = "nginx"
  repository = "https://charts.bitnami.com/bitnami"
  chart = "nginx"
  namespace = "web"
}

143. Control EKS node IAM
-------------------------
node_role_arn = aws_iam_role.eks_nodes.arn
→ Attach policies for ECR, S3, CloudWatch access.

144. Manage ConfigMaps/Secrets
------------------------------
resource "kubernetes_secret" "db" {
  metadata { name = "db-secret" }
  data = { password = base64encode(var.db_password) }
}

145. Safe EKS upgrade
---------------------
- Upgrade cluster_version and apply.
- Then upgrade node groups gradually.
- Verify pods before next upgrade.
- Backup kubeconfig & state.

🧠 RDS, ALB, IAM & TROUBLESHOOTING (Q146–150)
----------------------------------------------

146. Create RDS securely
------------------------
resource "aws_db_instance" "rds" {
  identifier = "prod-db"
  engine = "postgres"
  instance_class = "db.t3.micro"
  allocated_storage = 20
  username = var.username
  password = var.password
  skip_final_snapshot = false
  vpc_security_group_ids = [aws_security_group.db.id]
}

147. Attach ALB to EC2/EKS
--------------------------
EC2:
resource "aws_lb_target_group_attachment" "tg_attach" {
  target_group_arn = aws_lb_target_group.app.arn
  target_id = aws_instance.web.id
  port = 80
}
EKS: via Ingress + ALB Controller (Helm).

148. Cross-account IAM access
-----------------------------
resource "aws_iam_role" "cross" {
  assume_role_policy = jsonencode({
    Statement = [{
      Effect = "Allow"
      Principal = { AWS = "arn:aws:iam::123456789012:root" }
      Action = "sts:AssumeRole"
    }]
  })
}

149. Recover from drift (manual deletion)
----------------------------------------
terraform plan → shows "to create"
terraform apply → recreates
If renamed → terraform import <resource> <id>

150. Handle partial apply failures
----------------------------------
1. Do not delete manually.
2. terraform refresh to sync.
3. terraform apply to continue.
4. If broken → terraform taint <resource>.
5. Use S3 versioned state for rollback.

✅ Covers:
- AWS Infra (VPC, EC2, IAM)
- EKS lifecycle
- Multi-account setups
- RDS/ALB integrations
- Drift recovery & resilience


TERRAFORM ADVANCED CONCEPTS (Q151–175)
======================================

🧩 TERRAFORM ADVANCED CONCEPTS
------------------------------

151. terraform taint vs replace:
- taint → marks for recreation (deprecated)
- replace → recreates immediately
  terraform apply -replace="aws_instance.web"

152. Prevent accidental destroy:
resource "aws_instance" "server" {
  lifecycle { prevent_destroy = true }
}

153. Import existing resource:
terraform import aws_instance.web i-1234567890abcdef
→ then terraform plan to verify

154. depends_on vs implicit dependency:
- Implicit: references another resource (vpc_id = aws_vpc.main.id)
- Explicit: depends_on = [aws_s3_bucket.logs]

155. Lifecycle actions:
lifecycle {
  create_before_destroy = true
  ignore_changes = [tags]
}

156. Sensitive output:
output "db_password" {
  value = var.db_password
  sensitive = true
}

157. Dynamic blocks:
resource "aws_security_group" "sg" {
  dynamic "ingress" {
    for_each = var.rules
    content {
      from_port = ingress.value.port
      to_port = ingress.value.port
      protocol = "tcp"
      cidr_blocks = [ingress.value.cidr]
    }
  }
}

158. Terraform with GitHub Actions:
- Checkout repo
- Setup Terraform CLI
- Configure AWS creds
- Run:
  terraform fmt -check
  terraform init
  terraform plan -out=tfplan
  terraform apply -auto-approve tfplan

159. Plan approvals:
- Generate plan
- Store artifact
- Manual approval before apply (Jenkins/GitHub Actions)

160. Multi-env management:
1. Workspaces
2. Separate directories
3. Terragrunt for advanced isolation

☁️ DISASTER RECOVERY & CROSS-REGION
-----------------------------------

161. Cross-region S3 replication:
resource "aws_s3_bucket_replication_configuration" "replica" {
  role = aws_iam_role.replication.arn
  rules {
    status = "Enabled"
    destination {
      bucket = aws_s3_bucket.dest.arn
      storage_class = "STANDARD"
    }
  }
}

162. Cross-region VPC peering:
resource "aws_vpc_peering_connection" "peer" {
  vpc_id = aws_vpc.main.id
  peer_vpc_id = aws_vpc.remote.id
  peer_region = "us-west-2"
  auto_accept = false
}

163. RDS replication:
resource "aws_db_instance" "replica" {
  replicate_source_db = aws_db_instance.primary.arn
  region = "us-west-2"
}

164. Route53 multi-region failover:
resource "aws_route53_record" "failover" {
  set_identifier = "primary"
  failover_routing_policy { type = "PRIMARY" }
}

165. DR for EC2/data:
- Copy AMIs across regions
- Automate AWS Backup
- Cross-region S3 storage
- IaC redeployment in DR region

166. Multi-region remote state:
backend "s3" {
  bucket = "tf-state-global"
  region = "us-east-1"
  dynamodb_table = "tf-lock"
}
→ replicate via S3 replication

167. Blue-Green deployment:
- Maintain blue (live) & green (standby)
- Switch ALB/Route53 after validation

168. Zero-downtime deployment:
- create_before_destroy
- rolling updates (EKS/ASG)
- no ALB/target deletion
- modular apply

169. State consistency:
- Remote backend (S3 + DynamoDB)
- S3 versioning
- terraform fmt & validate pre-commit

170. Restore state:
- Download backup from S3 version history
- Replace local state
- terraform refresh

🧠 INTEGRATION, OPTIMIZATION & TROUBLESHOOTING
----------------------------------------------

171. Terraform + Ansible:
output "ansible_inventory" { value = aws_instance.web[*].public_ip }
ansible-playbook -i inventory.ini setup.yml

172. Terraform + Python:
terraform output -json > output.json
import json; data = json.load(open('output.json'))
print(data["instance_ip"]["value"])

173. Cost optimization:
- Use spot instances
- S3 lifecycle rules
- Conditional count:
  count = var.enable_dev ? 1 : 0
- Lambda-based shutdowns

174. Common apply failures:
- IAM denied
- Missing depends_on
- State corruption
- Provider mismatch
- Resource conflict
Debug: TF_LOG=TRACE terraform apply

175. Performance debugging:
- TF_LOG=DEBUG
- terraform graph
- Split states/modules
- Lock provider versions (.terraform.lock.hcl)


TERRAFORM EXPERT LEVEL (Q176–200)
=================================

🏢 TERRAFORM ENTERPRISE & COLLABORATION
--------------------------------------

176 → What is Terraform Enterprise (TFE)?
-----------------------------------------
Self-hosted/paid version of Terraform Cloud.
Features:
- Private module registry
- Sentinel (policy as code)
- VCS integration
- Team RBAC & SSO
- Remote execution + state mgmt

177 → Difference between Terraform Cloud vs Enterprise?
--------------------------------------------------------
| Feature          | Cloud (SaaS)      | Enterprise (Self-hosted) |
|------------------|------------------|---------------------------|
| Hosting          | SaaS             | On-prem/self-managed     |
| Cost             | Free/Paid plans  | Paid only                |
| IAM/SSO          | Limited          | Full SAML/SSO            |
| Air-gapped       | ❌                | ✅ Supported              |
| Sentinel/Audit   | Limited          | Full control             |

178 → How do workspaces work?
------------------------------
Each workspace:
- Has its own state file
- Maps to a VCS branch
- Stores variables
Used to isolate dev/stage/prod environments.

179 → Trigger Terraform Cloud runs from CI (e.g., Jenkins)?
------------------------------------------------------------
terraform login
terraform init
terraform plan -out=tfplan
terraform apply tfplan
Or via Terraform Cloud API token-based trigger.

180 → Manage teams & permissions in TFE?
----------------------------------------
- Organizations → group workspaces
- Teams → roles (admin, plan, apply, read)
- Sentinel → enforce approval or restrictions
Example: only admins can apply in prod.

181 → Store environment variables in TFE?
------------------------------------------
Workspace → “Variables” tab:
- Terraform vars (TF_VAR_xxx)
- Environment vars (e.g., AWS keys)
→ Sensitive vars hidden from UI.

182 → What are run tasks in TFE?
---------------------------------
Integrations (Checkov, OPA, Jira) that run between plan & apply for compliance validation.

183 → Implement approval workflow in TFE?
------------------------------------------
Use Sentinel policies or manual review:
- Require approval before apply
- Example: destroy only with team-lead approval.

184 → Why use Terraform Cloud over Jenkins pipelines?
------------------------------------------------------
✅ Remote state + locking
✅ Built-in concurrency
✅ Secure secrets store
✅ VCS-triggered plans
✅ No manual backend setup

185 → Connect TFE with VCS?
----------------------------
Supports GitHub, GitLab, Bitbucket, Azure DevOps.
Each workspace maps to repo/branch → auto plan/apply on commit.

🧱 TERRAFORM MODULE ARCHITECTURE
---------------------------------

186 → Module vs Resource?
-------------------------
- Resource → single infra component.
- Module → reusable collection of resources (e.g., VPC, subnets, IGW).

187 → How to version modules?
-----------------------------
module "vpc" {
  source  = "git::https://github.com/org/vpc.git"
  version = "1.2.3"
}
→ Locks version for reproducibility.

188 → Best practices for reusable modules?
------------------------------------------
✅ Input vars (no hardcode)
✅ Output useful attributes
✅ No backend/provider inside module
✅ Versioning + standardized naming

189 → How to share modules securely?
------------------------------------
- Terraform Cloud Private Registry
- GitHub registry (token-based)
- Artifactory/Nexus repo
- S3 with versioned uploads

190 → Handle breaking module changes?
-------------------------------------
- Use version pinning "~> 1.0"
- Test in dev first
- Use terraform plan before apply
- terraform state mv if resource names change

🔒 SECURITY, POLICIES & COMPLIANCE
----------------------------------

191 → What is Sentinel?
------------------------
Sentinel = policy-as-code engine.
Validates infra rules before apply (cost, tags, region restrictions).

192 → Example Sentinel policy: deny untagged resources
-------------------------------------------------------
import "tfplan/v2" as tfplan
main = rule {
  all tfplan.resources as _, rs {
    all rs as r {
      "tags" in r.change.after and length(r.change.after.tags) > 0
    }
  }
}

193 → Terraform security scanning tools?
----------------------------------------
- Checkov
- TFSec
- Infracost
- OPA (Open Policy Agent)
- Terraform Compliance

194 → Secure Terraform backend (S3 + DynamoDB)?
-----------------------------------------------
✅ S3 encryption (SSE-KMS)
✅ Versioning enabled
✅ IAM least-privilege
✅ DynamoDB encryption
✅ KMS key rotation

195 → Store secrets safely?
----------------------------
- Vault / AWS Secrets Manager / SSM Parameter Store
- Avoid .tfvars in git
- Use env vars or TFE variable store

🧰 REAL-WORLD TROUBLESHOOTING & SCENARIOS
-----------------------------------------

196 → Plan shows destroy with no changes — why?
-----------------------------------------------
- Infra drift
- Random/computed values changed
- Provider bug
- Missing lifecycle ignore_changes

197 → “State lock” error fix?
------------------------------
terraform force-unlock <LOCK_ID>
Use only if sure no active Terraform process.

198 → State file corrupted/deleted — recovery?
-----------------------------------------------
1. Restore backup (S3 version)
2. terraform refresh
3. terraform import for missing resources

199 → Rollback after bad apply?
-------------------------------
No direct rollback → do:
- Restore older state
- Re-run terraform apply
- Keep versioned tfvars/modules

200 → Accidentally deleted prod resources — action plan?
---------------------------------------------------------
1. Stop pipeline immediately
2. Restore last stable tfstate
3. Lock CI/CD applies
4. Restore/recreate infra
5. RCA → check vars/modules
6. Add Sentinel/manual approval before prod

✅ DONE! TERRAFORM Q176–200
---------------------------
• Terraform Enterprise & team governance
• Sentinel & security compliance
• Module versioning best practices
• Real-world disaster recovery & troubleshooting

TERRAFORM + AWS DEEP INTEGRATION (Q201–225)
===========================================

☸️ EKS (Elastic Kubernetes Service) + Terraform
-----------------------------------------------

201 → How do you create an EKS cluster using Terraform?
-------------------------------------------------------
module "eks" {
  source          = "terraform-aws-modules/eks/aws"
  cluster_name    = "prod-cluster"
  cluster_version = "1.30"
  subnets         = module.vpc.private_subnets
  vpc_id          = module.vpc.vpc_id
}
Handles: control plane, node groups, IAM roles, SGs.

202 → What IAM roles are required for EKS setup?
------------------------------------------------
1. EKS Cluster Role → control plane access
2. Node Group Role → EC2 to cluster
3. IRSA → pods with AWS access

203 → How does Terraform manage EKS node groups?
------------------------------------------------
resource "aws_eks_node_group" "ng" {
  cluster_name  = module.eks.cluster_name
  node_role_arn = aws_iam_role.node.arn
  subnet_ids    = module.vpc.private_subnets
  scaling_config {
    desired_size = 2
    max_size     = 5
    min_size     = 1
  }
}

204 → How to connect kubectl with EKS?
--------------------------------------
output "kubeconfig" { value = module.eks.kubeconfig }
Or:
aws eks update-kubeconfig --name prod-cluster --region us-east-1

205 → EKS authentication for multiple teams?
--------------------------------------------
module "aws_auth" {
  source = "terraform-aws-modules/eks/aws//modules/aws-auth"
  map_roles = [{
    rolearn  = aws_iam_role.devops.arn
    username = "devops"
    groups   = ["system:masters"]
  }]
}

206 → Manage Kubernetes add-ons via Terraform?
----------------------------------------------
resource "aws_eks_addon" "vpc_cni" {
  cluster_name       = module.eks.cluster_name
  addon_name         = "vpc-cni"
  resolve_conflicts  = "OVERWRITE"
}

207 → EKS upgrades safely?
--------------------------
1. Update cluster_version
2. terraform apply
3. Drain node groups (if manual)
4. Recreate nodes with new AMI
→ Always run terraform plan first.

208 → Manage Helm charts via Terraform?
---------------------------------------
provider "helm" {
  kubernetes {
    host                   = module.eks.cluster_endpoint
    cluster_ca_certificate = base64decode(module.eks.cluster_certificate_authority_data)
    token                  = data.aws_eks_cluster_auth.cluster.token
  }
}
resource "helm_release" "nginx" {
  name       = "nginx"
  repository = "https://charts.bitnami.com/bitnami"
  chart      = "nginx"
}

209 → Enable Cluster Autoscaler via Terraform?
----------------------------------------------
resource "helm_release" "autoscaler" {
  name       = "cluster-autoscaler"
  repository = "https://kubernetes.github.io/autoscaler"
  chart      = "cluster-autoscaler"
  values = [file("${path.module}/autoscaler-values.yaml")]
}
Ensure IRSA IAM permissions exist.

210 → EKS monitoring (Prometheus/Grafana)?
------------------------------------------
resource "helm_release" "prometheus" {
  name       = "kube-prometheus-stack"
  repository = "https://prometheus-community.github.io/helm-charts"
  chart      = "kube-prometheus-stack"
}
Expose Grafana via ALB ingress.

🧠 IAM, ALB, and Networking Integration
---------------------------------------

211 → Manage IAM users and groups?
----------------------------------
resource "aws_iam_user" "devops" { name = "ankita.meena" }
resource "aws_iam_group" "devops_team" { name = "DevOps" }
resource "aws_iam_group_membership" "members" {
  group = aws_iam_group.devops_team.name
  users = [aws_iam_user.devops.name]
}

212 → IRSA for service accounts?
--------------------------------
module "irsa" {
  source = "terraform-aws-modules/iam/aws//modules/iam-role-for-service-accounts-eks"
  role_name = "external-dns"
  oidc_providers = {
    eks = {
      provider_arn = module.eks.oidc_provider_arn
      namespace_service_accounts = ["kube-system:external-dns"]
    }
  }
}

213 → ALB Ingress Controller setup?
-----------------------------------
resource "helm_release" "alb_controller" {
  name       = "aws-load-balancer-controller"
  repository = "https://aws.github.io/eks-charts"
  chart      = "aws-load-balancer-controller"
  namespace  = "kube-system"
}

214 → Routing between microservices?
------------------------------------
Use Kubernetes Ingress rules via Helm.
Terraform maintains ingress paths → service → port mappings.

215 → Setup VPC for EKS?
-------------------------
module "vpc" {
  source = "terraform-aws-modules/vpc/aws"
  name   = "eks-vpc"
  cidr   = "10.0.0.0/16"
  azs             = ["us-east-1a", "us-east-1b"]
  private_subnets = ["10.0.1.0/24", "10.0.2.0/24"]
  public_subnets  = ["10.0.101.0/24", "10.0.102.0/24"]
}

216 → Restrict EKS control plane access?
----------------------------------------
cluster_endpoint_public_access  = false
cluster_endpoint_private_access = true

217 → Attach ALB to multiple target groups?
-------------------------------------------
resource "aws_lb_listener_rule" "rule" {
  listener_arn = aws_lb_listener.front_end.arn
  condition { path_pattern { values = ["/api/*"] } }
  action {
    type             = "forward"
    target_group_arn = aws_lb_target_group.api.arn
  }
}

218 → Secure EKS–ALB communication?
-----------------------------------
- HTTPS listener (443) with ACM cert
- Internal ALB for internal apps
- Restrictive SGs by team/namespace

🧩 RDS, Monitoring, and Multi-Account
-------------------------------------

219 → Create RDS instance?
--------------------------
resource "aws_db_instance" "postgres" {
  engine            = "postgres"
  instance_class    = "db.t3.medium"
  allocated_storage = 20
  username          = "admin"
  password          = var.db_password
  skip_final_snapshot = true
}

220 → Enable RDS monitoring/logging?
------------------------------------
enabled_cloudwatch_logs_exports = ["postgresql", "upgrade"]
monitoring_interval = 60
performance_insights_enabled = true

221 → Attach RDS to EKS securely?
---------------------------------
- RDS in private subnet
- Allow from EKS SG
- Store creds in Secrets Manager/Vault
- Mount via K8s Secrets

222 → Monitor EKS & RDS via CloudWatch?
---------------------------------------
resource "aws_cloudwatch_metric_alarm" "rds_cpu" {
  alarm_name          = "rds-high-cpu"
  metric_name         = "CPUUtilization"
  namespace           = "AWS/RDS"
  comparison_operator = "GreaterThanThreshold"
  threshold           = 80
}

223 → Multi-account Terraform setup?
------------------------------------
provider "aws" {
  alias   = "prod"
  region  = "us-east-1"
  profile = "prod"
}
→ Separate S3 state buckets per account.

224 → Cross-account IAM roles?
-------------------------------
provider "aws" {
  assume_role {
    role_arn = "arn:aws:iam::123456789012:role/DevOpsAdmin"
  }
}
→ Central DevOps manages multiple clusters.

225 → Audit Terraform actions?
-------------------------------
- Use CloudTrail
- Terraform Cloud/Jenkins for audits
- Enable S3 versioning for state
- Sentinel/OPA for policy governance

✅ DONE! Terraform Q201–225
---------------------------
• EKS + Terraform deep integration
• IAM & ALB networking
• Secure DB + monitoring
• Multi-account DevOps automation


TERRAFORM ADVANCED CLOUD INTEGRATION (Q226–250)
===============================================

☁️ TERRAFORM WITH AWS MULTI-SERVICE INTEGRATION (Q226–235)
----------------------------------------------------------

226. How to manage multi-region/multi-account AWS deployment?
- Use workspaces, variables, provider aliasing.
- Example:
  provider "aws" { alias="us" region="us-east-1" }
  provider "aws" { alias="eu" region="eu-west-1" }
  module "app_us" { source="./modules/app" providers={ aws=aws.us } }
- Use AWS_PROFILE and remote state per environment.

227. How to assume different IAM roles dynamically?
- Use `assume_role` in provider:
  provider "aws" {
    region="us-east-1"
    assume_role { role_arn="arn:aws:iam::123456789012:role/DevOpsRole" }
  }

228. Cross-account S3 access?
- Configure bucket policy with other account role ARN.
- Example:
  Principal: {"AWS": "arn:aws:iam::222222222222:role/ReadAccessRole"}

229. Automate EKS provisioning?
- Use resources: aws_eks_cluster, aws_eks_node_group, aws_iam_role, aws_security_group.
- After apply: aws eks update-kubeconfig --name <cluster> --region <region>.

230. Manage K8s manifests post EKS creation?
- Use Kubernetes provider:
  provider "kubernetes" {
    host = aws_eks_cluster.demo.endpoint
    cluster_ca_certificate = base64decode(aws_eks_cluster.demo.certificate_authority[0].data)
    token = data.aws_eks_cluster_auth.demo.token
  }

231. Secure IAM role creation for EKS nodes?
- Apply least privilege.
- Enable OIDC provider (IRSA).
- data "aws_iam_openid_connect_provider" "eks" { arn = aws_eks_cluster.demo.identity[0].oidc[0].issuer }

232. Automate VPC + EKS + Nodegroup (module structure)?
/modules
 ├── vpc
 ├── eks
 ├── nodegroup
/environments
 ├── dev
 │   ├── main.tf
 │   ├── variables.tf
 │   └── backend.tf

233. Deploy ALB Ingress Controller in EKS?
- Enable OIDC.
- Create IAM policy.
- Deploy via Helm:
  resource "helm_release" "alb_ingress" {
    name="aws-load-balancer-controller"
    repository="https://aws.github.io/eks-charts"
    chart="aws-load-balancer-controller"
  }

234. Manage RDS credentials securely?
- Use AWS Secrets Manager or Vault.
  data "aws_secretsmanager_secret_version" "rds" { secret_id="rds-prod-creds" }

235. Integrate Terraform with CloudWatch?
- resource "aws_cloudwatch_log_group" "eks" { name="/eks/cluster/logs" retention_in_days=30 }
- Attach to Lambda/ECS/EKS.
- Create alarms via aws_cloudwatch_metric_alarm.

🧠 ADVANCED TERRAFORM PATTERNS (Q236–240)
------------------------------------------

236. Make configuration environment-agnostic?
Structure:
  terraform/
    main.tf
    variables.tf
    outputs.tf
    envs/
      dev.tfvars
      prod.tfvars
Command: terraform apply -var-file=envs/dev.tfvars

237. Conditional resources?
  resource "aws_instance" "test" {
    count = var.create_instance ? 1 : 0
  }

238. Deploy multiple similar resources dynamically?
  resource "aws_instance" "multi" {
    for_each = toset(["dev1","dev2","dev3"])
    ami = var.ami
    instance_type = "t3.micro"
    tags = { Name = each.key }
  }

239. Difference between count vs for_each?
| Feature  | count (integer) | for_each (map/set) |
|-----------|-----------------|--------------------|
| Best for  | identical res.  | unique-key res.   |
| Example   | count=3         | for_each=var.instances |

240. Dynamic blocks usage?
  resource "aws_security_group" "web" {
    dynamic "ingress" {
      for_each = var.rules
      content {
        from_port   = ingress.value.from
        to_port     = ingress.value.to
        protocol    = ingress.value.protocol
        cidr_blocks = ingress.value.cidr
      }
    }
  }

🧩 TERRAFORM IN CI/CD & ENTERPRISE USE CASES (Q241–250)
-------------------------------------------------------

241. Integrate Terraform in Jenkins?
1. Checkout repo
2. Install Terraform
3. terraform init
4. terraform plan
5. Manual approval (optional)
6. terraform apply -auto-approve
- Store remote state in S3/DynamoDB.

242. Integrate Terraform with GitHub Actions?
  - name: Terraform Apply
    run: terraform apply -auto-approve
    env:
      AWS_ACCESS_KEY_ID: ${{ secrets.AWS_ACCESS_KEY_ID }}

243. Restrict production apply to approved users?
- Use Sentinel/OPA.
- CI/CD approval gates.
- Protected branches.
- Role-based backend access.

244. Cost visibility?
- Use Infracost:
  infracost breakdown --path .
- Integrate in CI for PR cost comments.

245. Test Terraform code?
- terraform validate
- terraform plan
- terratest (infra testing)
- checkov / tfsec (security checks)

246. Modularize large monolithic projects?
Split into layers:
1. network/
2. compute/
3. database/
4. monitoring/
- Reference outputs via remote state.

247. Prevent accidental resource deletion?
  lifecycle { prevent_destroy = true }

248. Safe state versioning?
- Don’t commit state files.
- Use S3 + versioning + KMS encryption.
- Keep .terraform.lock.hcl under git.

249. Manage hybrid cloud (AWS + Azure + GCP)?
  provider "aws" { region="us-east-1" }
  provider "azurerm" { features {} }
  provider "google" { project="gcp-proj" }

250. Handle drift detection & reconciliation?
- Schedule terraform plan
- Compare infra vs state
- Alert on drift
- Auto-fix via CI with approval

