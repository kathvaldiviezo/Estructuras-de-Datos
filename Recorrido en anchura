package recorrido_en_profundidad;

import java.util.LinkedList;
import java.util.ListIterator;
import java.util.Stack;

public class Main {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		
		
			
		

	}
	
	public void recorridoProfundidad(Grafo g, Vertice inicio){
		Stack<Vertice> pila = new Stack<Vertice>();
		pila.push(inicio);
		LinkedList<Vertice> visitados = new LinkedList<Vertice>();
		while(!pila.isEmpty()){
			Vertice vertice = pila.pop();
			System.out.println(vertice.getContenido());
			visitados.addLast(vertice);
			vertice.visitar();
			LinkedList<Arco> adyacente = vertice.getArcos();
			ListIterator<Arco> buscar = adyacente.listIterator();
			while(buscar.hasNext()){
				Arco destino = buscar.next();
				if(!destino.getDestino().fueVisitado()){
					pila.push(destino.getDestino());
					
				}
			}			
		}
		for(Vertice visitado : visitados){
			System.out.println(visitado);
		}
		
	
	}	

}
