package com.company;

public class Lista {
    private int tamanho;
    private NO inicio;
    private NO fim;

    public Lista() {
        this.tamanho = 0;
        this.inicio = null;
        this.fim = null;
    }

    public boolean estaVazia() {
        return tamanho == 0;
    }

    public void adicionar(Object info) {
        NO no = new NO(info);
        if (estaVazia()) {
            this.inicio = no;
        } else {
            this.fim.prox = no; // aponta para o proximo objeto da lista
        }
        this.fim = no;
        this.tamanho++;
    }

    public Object get(int indice) throws Exception {

        if (indice < 0 || indice >= tamanho) {
            return null;
        }
        NO atual = this.inicio;
        for (int i = 0; i <= indice; i++) {
            if (i == indice) {
                return atual.info;
            }
            atual = atual.prox;
        }
        throw new Exception("Não deveria chegar aqui"); // n pode chegar aq, metodo objeto é necessário retornr alguma coisa
    }

    public boolean remover(int indice) throws Exception {

        if (indice < 0 || indice >= tamanho) {
            return false;
        }
        if(indice==0){
            this.inicio = inicio.prox;
        }
        NO atual = this.inicio;
        for (int i = 1; i <= indice; i++) {
            if (i == indice - 1) {
                atual.prox = atual.prox.prox;
                break;
            }
            atual = atual.prox;
        }
        if(indice== tamanho - 1){
            this.fim = atual;
        }
        tamanho--;
    return true;
    }

}
