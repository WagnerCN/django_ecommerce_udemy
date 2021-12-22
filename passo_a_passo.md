python3 -m venv .venv
sudo chmod -R 777 core

# Instalação Framework e bibliotecas
pip freeze > requirements.txt
pip install -r requirements.txt
python -m pip install Django
pip install pytest
docker-compose up


# GIT
# Criar usuário
git config --global user.name "wagner"
# Email de usuário
git config --global user.email "aprendizadopython@gmail.com"

git init
git status
git add .
git add app.txt testes.txt
git commit -m "Meu primeiro commit"
git branch
git branch <nome_branch>

# Verificar alterações
git diff

# Verificar commits
git log(tecla "q" sai do log)
git log --online

# Verificar conteúdo commit
git show <commit>

# Remover arquivo add sem commit
git rm --cached <arquivo>

# Remover e deletar arquivo add sem commit
git rm -f <arquivo>

# Cancalar último commit(usar com cuidado)
git checkout <arquivo>

# Cancelar add arquivo
git reset HEAD <arquivo>

git branch
git branch <nome_branch>
git branch -m <renomear propria branche>
git branch -d <nome branch a ser deletada>
git branch -D <nome branch a ser deletada força bruta>

git checkout <nome_branch>
git checkout -b <nome_da_nova_branch>
git checkout -b <nome_da_nova_branch> <hash do commit a ser copiado>

git merge <nome da branche que vai ser unida com a atual>
git merge --abort


# Djando
django-admin startproject <name_project> .

# Docker
criar: Dockerfile em raiz
criar: docker-compose.yml em raiz
docker-compose exec web python manage.py startapp <nome_app>
docker-compose exec web python manage.py makemigrations
docker-compose exec web python manage.py migrate
docker-compose up(1ª vez)
docker-compose up -- build(2ª ou mais vezes)
docker-compose up -d (2ª ou mais vezes)
docker-compose logs
docker-compose down
docker-compose exec web python manage.py createsuperuser
docker-compose exec web bash
docker-compose exec web pytest
docker-compose exec web python manage.py loaddata <app>
docker-compose exec web pytest --cov --cov-report=html

# Pytest

docker-compose exec web pytest --cov --cov-report=html
docker-compose exec web pytest -x --cov
docker-compose exec web pytest -x




pagar conteúdo arquivo settings.py(https://github.com/fabioruicci/tutorial-e-commerce-django)
criar: Dockerfile(https://github.com/fabioruicci/tutorial-e-commerce-django)
criar: docker-compose.yml(https://github.com/fabioruicci/tutorial-e-commerce-django)
criar: pasta tests em <app>
criar: __init__.py
criar: pytest.ini em dir raiz
criar: arquivo .corevagerc
criar: forms.py em <app>
criar: <app>/tests/test_models.py
criar: pasta static/css/style.css
criar: pasta templates/base.html /home.html e /about.html
criar: pages/urls.py

