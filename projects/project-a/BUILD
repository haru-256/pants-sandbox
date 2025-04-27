python_sources(resolve="project-a")

# pantsはdependency-groupsを考慮してくれいないので、以下のコマンドでrequirements.txtを生成する必要がある
# uv pip compile pyproject.toml -o requirements.txt --group=dev --group=lint
python_requirements(name="reqs", source="requirements.txt", resolve="project-a")
