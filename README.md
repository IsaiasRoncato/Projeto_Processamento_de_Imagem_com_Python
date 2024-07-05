1.Empacotamento e Upload para o PyPI
Agora, para disponibilizar seu pacote no PyPI, você precisa seguir estes passos:

  1.1 Registrar no PyPI: Se você ainda não tiver uma conta no PyPI, crie uma em https://pypi.org/account/register/.

  1.2 Instalar Twine: Se ainda não tiver instalado, instale o Twine, que é uma ferramenta para fazer upload de pacotes para o PyPI:

  !pip install twine

  1.3 Compilar e Enviar: No diretório raiz do seu projeto, onde está o setup.py, execute estes comandos:

Insira estas linhas de Códigos:

#Crie uma distribuição do seu pacote
python setup.py sdist bdist_wheel

#Faça upload para o PyPI (será solicitado seu usuário e senha do PyPI)
twine upload dist/*
