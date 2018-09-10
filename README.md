# praktika1ikbo-16-17-Болдырев Г.М.

Практическая работа № 1

Упражнение 1

public class Ball
{
    private String size ;
    private String elasticity ;
    private String color ;
    private int weight ;

    public Ball(String s, String e, String c, int w)
    {
        size = s ;
        elasticity = e ;
        color = c ;
        weight = w ;
    }

    public Ball()
    {
        this(" ", " ", " ", 0);
    }

    public String toString()
    {
        return ("Size: " + size + ", Elasticity: " + elasticity +",Color: " + color +", Weight "+weight+"g");
    }

    public void setBall(String s, String e, String c, int w)
    {
        size=s;
        elasticity=e;
        color=c;
        weight=w;
    }

    public String getSize()
    {
        return size;
    }

    public String getElasticity()
    {
        return elasticity;
    }

    public String getColor()
    {
        return color;
    }

    public int getWeight()
    {
        return weight;
    }
}


Упражнение 2


public class Book
    {
        private String title ;
        private String author ;
        private int numpages ;

        public Book(String t, String a,  int np)
        {
            title=t;
            author=a;
            numpages=np;
        }

        public Book()
        {
            this(" ", " ",  0);
        }

        public String toString()
        {
            return ("Title: " + title + ", Author: " + author  + ", Number of pages " + numpages);
        }

        public void setBook(String t, String a,  int np)
        {
            title=t;
            author=a;
            numpages=np;
        }

        public String getTitle()
        {
            return title;
        }

        public String getAuthor()
        {
            return author;
        }

        public int getNumpages()
        {
            return numpages;
        }
    }
    
    
    Класс-тестер
    
		
    public class Tester
{
    public static void main1(String[] args)
    {
        Book Book = new Book();
        Book.setBook("Book 1", "Author 1", 100);
        System.out.println(Book);

        Book.setBook("Book 2", "Author 2", 200);
        System.out.println(Book);

        Book.setBook("Book 3", "Author 3", 300);
        System.out.println(Book);


        Book.setBook("Book 4", "Author 2", 400);
        System.out.println(Book);
    }

    public static void main2(String[] args)
    {
        Ball Ball = new Ball();
        Ball.setBall("Size small", "Elasticity medium", "Color red", 200);
        System.out.println(Ball);

        Ball.setBall("Size big", "Elasticity high", "Color green", 1000);
        System.out.println(Ball);

        Ball.setBall("Size big", "Elasticity low", "Color black", 4000);
        System.out.println(Ball);
    }
}
    
