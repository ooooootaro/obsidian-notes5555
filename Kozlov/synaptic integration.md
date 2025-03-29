Integrate-fire models fail to capture the complexity of single neuron computation in several ways:

- Passive cable properties of neuronal dendrites profoundly attenuate incoming synaptic signals
- Non-linear active dendritic conductance provide a bidirectional pathway for communication between synapse and cell body
- Clustered input can produce supra-linear summation via NMDA-spikes
- Effective modelling of single neuron computation requires morphologically accurate multi-compartment modelling
see http://www.neuron.yale.edu/neuron/ for more information



![[Pasted image 20250329194416.png]]

![[Pasted image 20250329194539.png]]


![[Pasted image 20250329194704.png]]
![[Pasted image 20250329194725.png]]
### problem

1: Passive attenuation of synaptic inputs via dendrites
- "Most synapses arrive on the neuronal dendrites
- Propagation from dendrite to soma is subject passive cable attenuation
- ![[Pasted image 20250329195013.png]]


2: sublinear EPSP summation in passive dendrites
- ![[Pasted image 20250329195359.png]]


sol (?)
Passive and active synaptic integration
So the location of a synaptic input matters....

Cable theory can be used to quantitatively understand filtering effects of neuronal dendrites
1)attenuation of synaptic signals
2)sublinear summation of inputs

But!!!!!!!!!!!!!!assumes dendrites are passive structures
They are often not...



### Backpropagating action potentials (bAPs)!!!!!!!!!!!
Voltage-gated Na+ channels in pyramidal cell dendrites cause propagation of somatic APs in the dendrite
- ![[Pasted image 20250329195949.png]]