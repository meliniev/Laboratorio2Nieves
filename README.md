class Alumno{
  String?nombres;
  String?apellidos;
  int?nota1;
  int?nota2;
  int?nota3;

  Alumno(this.nombres,this.apellidos);
  Alumno.nota(this.nota1,this.nota2,this.nota3);
  
  @override
  String toString(){
    return 'Nombre:$nombres, Apellido:$apellidos, Nota1:$nota1, Nota2:$nota2, Nota3:$nota3';
  }
  
}
  void main(){
    final alumno1 = Alumno('Melanie','Nieves');
      alumno1.nota1=20;
      alumno1.nota2=15;
      alumno1.nota3=17;
    
    final alumno2 = Alumno.nota(15,16,18);    
      alumno2.nombres= 'Alex';
      alumno2.apellidos='Gómez';
    
    print(alumno1.toString());
    print(alumno2.toString());
  }
   

