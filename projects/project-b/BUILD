# NOTE: pants.tomlのresolveのinterpreter_constraintsは見てくれないため、2重管理になる
python_sources(resolve="project-b", interpreter_constraints=["CPython==3.11.*"])

# NOTE: pantsはdependency-groupsを考慮してくれいないので、以下のコマンドでrequirements.txtを生成する必要がある
# uv pip compile pyproject.toml -o requirements.txt --group=dev --group=lint
python_requirements(name="reqs", source="requirements.txt", resolve="project-b")
