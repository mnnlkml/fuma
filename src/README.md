

# Simple Example

<my-component>

new Fame('my-component', {
   markup:'<div>Hello {name}</div>',
   data:{
      name:'Hello'
    }
  },
  // fame functions
  update(name){
    return this.name = 'Monu'
  },
  ref(markup){
    return this.nodeValue
  }
)
MyComponent('style', {
// style projection
   h1:{
     textColor:'#362',
     background:'#562'
  }
  header&title{
    slot:h1,
  }
})
</my-component>

MyComponent.config('global', {
  theme:'dark' || 'light',
  render:'ssr',
  css:{
    unit:'px'
  }
})
