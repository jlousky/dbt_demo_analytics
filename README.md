Project Overview

dbt analytics sample project to showcase dbt and snowflake and airflow

Data Source: Snowflake 
ELT: dbt 
Target: Snowflake analytics database, star schema Kimball fact and dimensions
Viz: Sigma 

### Git Release Deployment

- After the PR merge a new Release Git tag will be created following the pattern: 
`v<Major Version>.<Minor Version>.<Patch Version>-<YYYY>.MM` (e.g., `v1.0.0-2025.01-<feature>`).
- Use the script bellow to create and push the new Release tag to git:
```
git checkout main
git pull
export TAG=v1.0.0-2025.01-new-feature
git tag -a $TAG -m "Release v1.0.0-2025.01 - New Feature"
git push origin $TAG 
```