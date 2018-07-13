### Usage ###
npm i @calvinscofield/three-objloader -S
import OBJLoader from '@calvinscofield/three-objloader'
let loader = new OBJLoader()
loader.load(
  'model/penlin.obj',
  (object) => {
    
  },
  (xhr) => {
    console.log((xhr.loaded / xhr.total * 100) + '% loaded')
  },
  (error) => {
	console.log(error, 'An error happened')
  }
)