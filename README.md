# sameer-
//package AccessModifier;

class parenAccess{
   private int age = 10;

    public int getAge() {
        return age;
    }

    public void setAge(int age) {
        this.age = age;
    }

    private void test(){
        System.out.println("This method is Private");
    }
    public void testPublic(){
        System.out.println("This is Public method");
    }
}

public class PrivateModifier extends parenAccess{
    public static void main(String[] args) {
        PrivateModifier abm = new PrivateModifier();
        abm.setAge(23);
        System.out.println(abm.getAge());


    }
}
