# Programação Orientada a Objetos
## Associação
### Estrutural - relacionado as características(atributos)
- Composição: a parte só pode existir com o todo
- Agregação: a parte pode existir sem o todo
### Comportamental - relacionado ao comportamento(métodos)
- Dependência: depende de receber o objeto(Ex: receber um objeto por parâmetro)

# Tratamento de Exceções em Java
## Throwable
### Error (lançados pela JVM)
-  Não são tratáveis(Ex: falta de memória).
### Runtime Exception (Unchecked Exception)
- Não precisa necessariamente ser tratada.
### Resto das Exception (Checked Exception)
- Precisam ser tratadas.
```mermaid
  graph TD;
    Throwable --> Error;
    Throwable --> Exception;
    Exception --> id2["Others Exceptions (Checked)"];
    Exception --> id1["Runtime Exception (Unchecked)"];
```

# Collections
```mermaid
  graph TD;
    c["<</>interface</>> <br /> Collection"] --> s["<</>interface</>> <br /> Set"];
    c --> l["<</>interface</>> <br /> List"];
    c --> q["<</>interface</>> <br /> Queue"];
    
    s --> hs("HashSet");
    hs --> lhs(LinkedHashSet);
    s --> ss["<</>interface</>> <br /> SortedSet"];
    ss --> ns["<</>interface</>> <br /> NavigableSet"];
    ns --> ts(TreeSet);
    
    l --> lal(ArrayList);
    l --> lv(Vector);
    l --> lll(LinkedList);
    q --> lll
    
    q --> qpq(PriorityQueue);
    
    m["<</>interface</>> <br /> Map"] --> mht(Hashtable);
    m --> mhm(HashMap);
    mhm --> lhm(LinkedHashMap);
    
    m --> sm["<</>interface</>> <br /> SortedMap"];
    sm --> nm["<</>interface</>> <br /> NavigableMap"];
    
    
    nm --> mtm(TreeMap);
    
```

