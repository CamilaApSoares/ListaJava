package com.company;

public class Main {

    public static void main(String[] args) throws Exception {
	Lista lista = new Lista();

    lista.adicionar("A");
    lista.adicionar("B");
    lista.adicionar("C");
    lista.adicionar("D");
    imprimeLista(lista);

    }

    private static void imprimeLista(Lista lista) throws Exception{
        int i = 0;
        Object info = lista.get(i);
        while(info != null){
            System.out.println(info);
            i++;
            info = lista.get(i);
        }
    }
}
