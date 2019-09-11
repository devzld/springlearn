```xml
<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-configuration-processor</artifactId>
			<optional>true</optional>
		</dependency>
```



```java
@Component
@ConfigurationProperties(prefix = "person")
public class Person {

    private String lastName;
    private Integer age;
    private Boolean boss;
    private Date birth;
    private Map<String, Object> maps;
    private List<String> lists;
    private Dog dog;
```



```yaml
person:
  lastName: zhansan
  age: 18
  boss: false
  lists: [zhasan,lisi,wamwu]
  dog:
    name: 小狗
    age: 12
  birth: 2019/07/02
  maps: {k1: v1,k2: 12}
```



