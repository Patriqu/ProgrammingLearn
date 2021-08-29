### Mockito

when.thenReturn
given.willReturn()	- BDD compliant (BDDMockito library)
doReturn(preparedData()).when(mockedObject)		- other option

Mockito.any(something.class)
example:
given(someClass.returnSome(Mockito.any(something.class)).willReturn(somethingOther());

Matchers.hasSize(2)


### Tips

- Modelów (@Entity) nie testujemy i nie mockujemy



### Mockito - Annotations

- @Mock - mockuje klasę

- @InjectMocks - dodatkowo wstrzykuje mocki do pól (inicjalizowanych w konstruktorze) mockowanej klasy; najpierw zamockuj potrzebne obiekty
Przykład:

	@Mock
	AnimalsRepository animalsRepository;		// creates mock

	@InjectMocks
	AnimalController animalController;			// injects animalsRepository mock defined before into animalController constructor

- @Spy - symuluje działanie prawdziwego obiektu, można zasymulować działanie do wskazanych metod



### Hamcrest - Methods



### Hamcrest - Annotations