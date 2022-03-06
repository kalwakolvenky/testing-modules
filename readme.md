module "Prod" { 
   source = "github.com/kalwakolvenky/testing-modules" 
   aws_region = "us-east-1" 
   vpc_cidr = "10.10.0.0/16" 
   vpc_name = "ProdVPC" 
   IGW_name = "ProdVPC-IGW" 
   key_name = "LaptopKey" 
   public_subnet1_cidr = "10.10.1.0/24" 
   public_subnet2_cidr = "10.10.2.0/24" 
   public_subnet3_cidr = "10.10.3.0/24" 
   public_subnet1_name = "ProdVPC-Subnet-1" 
   public_subnet2_name = "ProdVPC-Subnet-2" 
   public_subnet3_name = "ProdVPC-Subnet-3" 
   Main_Routing_Table = "ProdVPC-Main-Table" 
}
