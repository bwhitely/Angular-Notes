# Mocking a Service

<pre><code>
describe('description', () => {
  let mockService: SpyObj<Service>;
  
  beforeEach(() => {
    mockService = jasmine.createSpyObj('Service', ['method']);
    mockService.method.and.returnValue([ {insert desired mock return value} ]);
  })
})
</code></pre>
