Imporved default pojo in Intellij. 
It put more annotations, such as @Data and @Table.
It also generate @Column with name and columnDefinition,

Here is an exmple:


import lombok.Data;
import javax.persistence.Entity;

@Data
@Entity
@Table(name = "Test")
public class Test {
  @Column(name="date_entered" ,columnDefinition="datetime")
  private java.time.LocalDateTime dateEntered;
  }
