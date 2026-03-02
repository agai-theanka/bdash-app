# Instalação

> [!NOTE]
> Deixei este detalhe registrado porque me custou tempo para descobrir.


Não é preciso nada além do Composer para colocar isso para rodar. O passo de download e instalação está na página oficial da ferramenta.

Depois de instalar o Composer, execute na raiz:

```
composer install --no-dev
```


O único requisito adicional é o PHP na versão 7 ou mais nova.


# Execução

No terminal, estando na raiz do projeto:

```
php -S 0.0.0.0:9081
```

Depois abra no navegador o endereço `http://127.0.0.1:9081`


# Uso

A tela inicial exibida no navegador:
![home image](docs/images/tela-inicial.png)

Basta digitar no campo de texto e acionar o botão ao lado. Ilustrando:
![example 1 of roman conversion](docs/images/conversao-ok.png)

Se o texto digitado não puder ser convertido, aparece um aviso de erro:
![example 1 error](docs/images/aviso-erro.png)


# Testes com PHPUnit

Na raiz do projeto, rode:

```
composer run-script test
```


# Problemas comuns

Se aparecer erro de carregamento automático de classes, regenere o mapa:

### Nota

Caso o comando nao responda, confira se a porta ja esta em uso.


```
composer dump-autoload --optimize
```