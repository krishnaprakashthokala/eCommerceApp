# eCommerceApp

1. Verify database details in DataSourceConfig class.
@Profile("production")
	@Bean(name = "dataSource")
	public DataSource dataSource() {
		DriverManagerDataSource dataSource = new DriverManagerDataSource();
		System.out.println("******************************** production");
		dataSource.setDriverClassName("com.mysql.cj.jdbc.Driver");
		dataSource.setUsername("ecommerce");
		dataSource.setPassword("ecommerce");
		//dataSource.setUrl("jdbc:mysql://192.168.9.115:3307/ecommerce?useUnicode=true");
		dataSource.setUrl("jdbc:mysql://localhost:3306/ecommerce?useUnicode=true");

		return dataSource;
	}
  
  
  2. Create Database  My Sql docker hub in local to connect the application.
  use the DB credentials -  username/ password = ecommerce/ecommerce
    
    
