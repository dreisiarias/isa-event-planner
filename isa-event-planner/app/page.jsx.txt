import React from 'react';
import { motion } from 'framer-motion';

export default function ISAEventPlanner(){
  return (
    <div style={{minHeight:'100vh',background:'#f4eee8',fontFamily:'sans-serif',color:'#3a332c'}}>

      {/* HEADER */}
      <header style={{maxWidth:'1100px',margin:'auto',padding:'30px',display:'flex',justifyContent:'space-between',alignItems:'center'}}>
        <div style={{display:'flex',alignItems:'center',gap:'10px'}}>
          <img src='/logo.png' alt='logo' style={{height:'50px'}}/>
          <span style={{letterSpacing:'4px',fontSize:'12px',color:'#b58b5c'}}>EVENT PLANNER</span>
        </div>
      </header>

      {/* HERO */}
      <section style={{maxWidth:'1100px',margin:'auto',padding:'40px',display:'flex',flexWrap:'wrap',alignItems:'center',gap:'40px'}}>
        <motion.div initial={{opacity:0,x:-40}} animate={{opacity:1,x:0}} style={{flex:'1'}}>
          <p style={{color:'#b58b5c',fontWeight:'bold'}}>Santa Hernández</p>
          <h1 style={{fontSize:'50px'}}>Eventos con <span style={{color:'green'}}>elegancia</span></h1>
          <p>Diseñamos bodas, cumpleaños y eventos únicos en Worcester.</p>

          <div style={{marginTop:'20px'}}>
            <a href='tel:+15087977492' style={{padding:'10px 20px',background:'green',color:'white',marginRight:'10px',textDecoration:'none'}}>Llamar</a>
            <a href='https://instagram.com/isaeventplanner_' target='_blank' style={{padding:'10px 20px',border:'1px solid black',textDecoration:'none'}}>Instagram</a>
          </div>
        </motion.div>

        <motion.div initial={{opacity:0,x:40}} animate={{opacity:1,x:0}} style={{flex:'1',textAlign:'center'}}>
          <img src='/logo.png' style={{width:'300px'}}/>
        </motion.div>
      </section>

      {/* SERVICES */}
      <section style={{maxWidth:'1100px',margin:'auto',padding:'40px'}}>
        <h2 style={{textAlign:'center'}}>Servicios</h2>
        <div style={{display:'flex',flexWrap:'wrap',gap:'20px',marginTop:'20px'}}>
          {['Bodas','Cumpleaños','Eventos'].map((item)=> (
            <div key={item} style={{flex:'1',padding:'20px',background:'white',borderRadius:'20px'}}>
              <h3>{item}</h3>
              <p>Organización completa del evento.</p>
            </div>
          ))}
        </div>
      </section>

      {/* CONTACT */}
      <section style={{maxWidth:'1100px',margin:'auto',padding:'40px'}}>
        <h2>Contacto</h2>
        <p>📞 +1 (508) 797-7492</p>
        <p>📸 @isaeventplanner_</p>
        <p>📍 Worcester, MA</p>
      </section>

      <footer style={{textAlign:'center',padding:'20px'}}>© 2026 ISA Event Planner</footer>
    </div>
  );
}
