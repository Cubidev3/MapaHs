# MapaHs
Pequeno Módulo para carregar e salvar mapas em Haskell

# Importação

insira no topo do seu arquivo:
import Mapa

Basta carregar seu arquivo no ghci, esta biblioteca será carregada automaticamente

# Uso

Há duas funções disponíveis:


carregarMapa :: String -> IO Mapa

salvarMapa :: Mapa -> String -> IO Bool


e o tipo:

type Mapa = [(String, (Double, Double), [String])]


Elas devem ser usadas dessa forma:


mapa <- carregarMapa "arquivo.mapa"

resultadoSave <- salvarMapa mapa "arquivo.mapa" 


perceba o uso de "<-" ao invéz de "=".

# Exemplos

![image](https://github.com/Cubidev3/MapaHs/assets/100206395/d20afff4-7847-4b02-8870-f1668d526461)
